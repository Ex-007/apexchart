<template>
    <div>
         <div class="lieChart">

            <!-- LINE CHART -->
             <h2>Line Chart</h2>
            <div class="main">
                <h2>Line Chart</h2>
                <apexchart
                type="line"
                :options="linechartOptions"
                :series="linechartSeries"
                />
            </div>

            <!-- BAR CHART -->
             <h2>Bar Chart</h2>
            <div class="main">
                <h2>Bar Chart</h2>
                <apexchart
                type="bar"
                :options="barchartOptions"
                :series="barchartSeries"
                />
            </div>

            <!-- PIE CHART -->
             <h2>Pie Chart</h2>
            <div class="main">
                <h2>Pie Chart</h2>
                <apexchart
                type="pie"
                :options="piechartOptions"
                :series="piechartSeries"
                />
            </div>

            <!-- AREA CHART -->
             <h2>Area Chart</h2>
            <div class="main">
                <h2>Area Chart</h2>
                <apexchart
                type="area"
                :options="areachartOptions"
                :series="areachartSeries"
                />
            </div>
         </div>
    </div>
</template>

<script setup>
    // LINE CHART
    const linechartSeries = ref([
        {
            name: "Sales",
            data: [11, 20, 30, 20, 50, 30]
        }
    ])
    const linechartOptions = ref({
        xaxis: {
            categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'June']
        }
    })

    // BAR CHART
    const barchartSeries = ref([
        {
            name: 'Revenue',
            data: [30, 20, 50, 32, 58, 45, 13],
        }
    ])

    const barchartOptions = ref({
        xaxis: {
            categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'June']
        }
    })

    // PIE CHARTS
    const piechartOptions = ref({
        labels: ['January', 'February', 'March']
    })
    const piechartSeries = ref([30, 50, 70])

        // AREA CHART
    const areachartSeries = ref([
        {
            name: "Sales",
            data: [11, 20, 30, 20, 50, 30]
        }
    ])
    const areachartOptions = ref({
        xaxis: {
            categories: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'June']
        },
        
    })





</script>

<style scoped>
    .lieChart{
        display: flex;
        padding: 24px;
        gap: 5px;
        align-items: center;
        justify-content: center;
        background-color: rgb(34, 34, 166);
        flex-direction: column;
    }
    .main{
        background-color: white;
        border-radius: 20px;
        padding: 5px;
    }
    .main h2{
        font-size: 10px;
    }
    h2{
        color: white;
    }
</style>