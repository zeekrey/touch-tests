<script lang="ts">
  const items = [...Array(8)]
</script>

<main class="w-screen bg-slate-50">
  <ul>
    {#each items as item, i}
      <li class="h-20 bg-slate-100 border-b border-b-slate-200">
        <button class="w-full h-full text-2xl text-slate-300 hover:bg-slate-600">
          {i} (only css:hover)
        </button>
      </li>
    {/each}
    {#each items as item, i}
      <li class="h-20 bg-amber-100 border-b border-b-amber-200">
        <button class="w-full h-full text-2xl text-amber-300 focus:bg-amber-600">
          {i} (only css:focus)
        </button>
      </li>
    {/each}
    {#each items as item, i}
    <li class="h-20 bg-red-100 border-b border-b-red-200">
      <button class="w-full h-full text-2xl text-red-300 active:bg-red-600">
        {i} (only css:active)
      </button>
    </li>
  {/each}
  </ul>
</main>

<style>
  
</style>