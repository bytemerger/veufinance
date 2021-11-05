<script>
import { Bar } from 'vue-chartjs'

export default {
  extends: Bar,
  name: "SpendingChart",
  data: () => ({
      chartData: {
        labels: ["May", "Jun", "Jul", "Aug", "Sept", "Oct", "Nov", "Dec", "Jan"],
        datasets: [{
          label: false,
          borderWidth: 0.5,
          borderRadius: 3,
          backgroundColor: [
            'rgba(255, 99, 132, 0.2)',
            'rgba(54, 162, 235, 0.2)',
            'rgba(255, 206, 86, 0.2)',
            'rgba(75, 192, 192, 0.2)',
            'rgba(153, 102, 255, 0.2)',
            'rgba(255, 159, 64, 0.2)',
            'rgba(255, 99, 132, 0.2)',
            'rgba(54, 162, 235, 0.2)',
            'rgba(255, 206, 86, 0.2)',
          ],
          borderColor: [
            'rgba(255,99,132,1)',
            'rgba(54, 162, 235, 1)',
            'rgba(255, 206, 86, 1)',
            'rgba(75, 192, 192, 1)',
            'rgba(153, 102, 255, 1)',
            'rgba(255, 159, 64, 1)',
            'rgba(255,99,132,1)',
            'rgba(54, 162, 235, 1)',
            'rgba(255, 206, 86, 1)',
          ],
          pointBorderColor: '#2554FF',
          data: [3000, 9880, 6000, 4500, 7000, 3500, 4000, 5000, 6500]
        }]
      },
      options: {
        scales: {
          yAxes: [{
            ticks: {
              stepSize: 4000,
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
          display: true
        },
        responsive: true,
        maintainAspectRatio: false,
        height: 300,
      }
  }),
  mounted () {
    this.renderChart(this.chartData, this.options)
  }
}
</script>

<style scoped>

</style>
