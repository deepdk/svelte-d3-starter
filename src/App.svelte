<script>
    const data = [
        { x: 155, y: 386, r: 20, fill: '#0000FF' },
        { x: 340, y: 238, r: 52, fill: '#FF0AAE' },
        { x: 531, y: 151, r: 20, fill: '#00FF88' },
        { x: 482, y: 307, r: 147, fill: '#7300FF' },
        { x: 781, y: 91, r: 61, fill: '#0FFB33' },
        { x: 668, y: 229, r: 64, fill: '#D400FF'}
    ];
</script>

<main>
    <svg width="1000" height="500">
        {#each data as {x,y,r,fill}}
        <circle 
           cx={x}
           cy={y}
           r={r}
           fill={fill}
           opacity={708/1000}
        />
        {/each}
    </svg>
</main>

<style>
    svg{
        background: #F3FFF0;
    }
</style>
