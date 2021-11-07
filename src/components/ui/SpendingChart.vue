<script>
import { Bar } from 'vue-chartjs'

export default {
  extends: Bar,
  name: "SpendingChart",
  data: () => ({
      chartData: {
        labels: ["May", "Jun", "Jul", "Aug", "Sept", "Oct", "Nov", "Dec", "Jan"],
        datasets: [{
          label: 'Spending',
          borderWidth: 0.2,
          barThickness: 1,
          borderRadius: 90,
          backgroundColor: [
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
          ],
          borderColor: [
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
            'rgb(203,231,240)',
            'rgb(23,28,40)',
          ],
          pointBorderColor: 'rgb(23,28,40)',
          data: [3000, 9880, 6000, 4500, 7000, 3500, 4000, 5000, 6500]
        }]
      },
      options: {
        scales: {
          yAxes: [{
            ticks: {
              stepSize: 2000,
              callback: function(value) {
                let values = value/1000;
                console.log(values)
                return '$' + values + 'K';
              }
            },
            gridLines: {
              display: false,
              drawBorder: false,
            },
          }],
          xAxes: [{
            gridLines: {
              display: false,
              drawBorder: false,
            }
          }]
        },
        legend: {
          display: false
        },
        tooltips: {
          callbacks: {
            label: function(tooltipItem) {
              console.log(tooltipItem)
              return tooltipItem.yLabel;
            }
          }
        },
        responsive: true,
        maintainAspectRatio: false,
      }
  }),
  mounted () {
    this.renderChart(this.chartData, this.options)
  }
}
</script>

<style scoped>

</style>
