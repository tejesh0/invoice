<script>
  import MoreMenu from './MoreMenu.svelte'
</script>

<div class="flex justify-between">
  <div>
    <button class="text-xxxs text-gray-500 font-medium border-2 py-1 px-2 mt-1 rounded-full">
      <span class="text-blue-400 mr-2">✉</span>DIRECT
    </button>
  </div>
  <div>
    <MoreMenu></MoreMenu>
    <div class="inline-block mr-1"></div>
    <button class="bg-blue-500 hover:bg-blue-700 text-xs text-white py-2 px-12 rounded border-2 border-blue-500">
      Approve
    </button>
  </div>
</div>
