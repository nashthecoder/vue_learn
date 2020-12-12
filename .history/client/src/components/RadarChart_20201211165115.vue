<script>
import { Radar } from "vue-chartjs";

export default {
  extends: Radar,
  data() {
    return {
      chartData: {
        labels: ["Crossfit", "Yoga", "Weightlifting", "Running", "Swimming"],
        datasets: [
          {
            borderWidth: 1,
            label: "My Workout",
            borderColor: ["rgba(255,99,132,1)"],
            backgroundColor: ["rgba(255, 99, 132, 0.2)"],
            data: [210, 399, 220, 234, 311]
          }
        ]
      },
      options: {
        legend: {
          display: true
        },
        responsive: true,
        maintainAspectRatio: false
      }
    };
  },
  mounted() {
    this.renderChart(this.chartData, this.options);
  }
};
</script>
