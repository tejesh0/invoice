<script>

  let menu, showMenu = false;

  function onClickOutside(event) {
    let target = event.target;
    let isOutside = true;
    while(target) {
      if (target === menu) {
        isOutside = false;
      }
      target = target.parentNode;
    }
    if (isOutside) {
      showMenu = false;
    }
  }
</script>

<style>
  .triangle {
    border: solid black;
    border-width: 0 2px 2px 0;
    padding: 2px;
    margin-top: 2px;
    transform: translate(0, -2px)rotate(45deg);
  }
</style>

<svelte:body on:click={onClickOutside}/>
<div class="relative inline-block" bind:this={menu}>
  <button on:click="{() => showMenu = !showMenu}" class="bg-gray-300 text-gray-900 text-xs py-2 px-4 rounded border-2 border-gray-400">
    More <i class="inline-block triangle"></i>
  </button>
  <div class="{showMenu ? 'block': 'hidden'} absolute right-0 mt-1 text-sm border-2 border-gray-300 w-56 z-10">
    <a class="block no-underline px-3 py-2" href="#">Export</a>
    <a class="block no-underline px-3 py-2" href="#">Mark as exported</a>
    <a class="block no-underline px-3 py-2" href="#">Setup Vendor</a>
    <a class="block no-underline px-3 py-2" href="#">Flag Invoice</a>
    <a class="block no-underline px-3 py-2" href="#">Archive Invoice</a>
    <a class="block no-underline px-3 py-2" href="#">Delete Invoice</a>
  </div>
</div>
