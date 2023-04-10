<template>
    <div class="graficaPie">
        <canvas ref="canvas"></canvas>
    </div>
</template>

<script>
import Chart from 'chart.js/auto';


export default {
  mounted() {
    this.renderChart();
  },
  methods: {
    renderChart() {
      const canvas = this.$refs.canvas;
      const context = canvas.getContext('2d');

      new Chart(context, {
        type: 'bar',
        data: {
          labels: [ '2020', '2021', '2022', '2023'],
          datasets: [
            {
              label: 'Rendimiento academico',
              data: [ 7.5, 8, 8.7, 8.3],
              backgroundColor: ["#FF6384",
                "#63FF84",
                "#84FF63",
                "#6384FF"],
              borderColor: 'rgba(54, 162, 235, 1)',
              borderWidth: 1,
            },
          ],
        },
        options: {
          scales: {
            yAxes: [
              {
                ticks: {
                  beginAtZero: true,
                },
              },
            ],
          },
        },
      });
    },
  },
};
</script>

<style>



</style>