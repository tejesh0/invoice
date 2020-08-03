<script>
  let snipView = false
</script>
<style>
  .triangle {
    border: solid black;
    border-width: 0px 8px 8px 0px;
    padding: 11px;
  }

  .down {
    transform: translate(-4.5px, -6px)scale(0.3)rotate(45deg);
  }

  .up {
    transform: translate(-4.5px, -4px)scale(0.3)rotate(225deg);
  }
</style>

<small class="{snipView ? 'hidden': 'block'} text-xxxs text-gray-500 font-bold">VENDOR</small>
<div class="flex items-center">
  <h1 class="inline-block mr-3 pt-1 text-xl">Freguesia Cheese</h1>
  <div on:click={()=> snipView = !snipView} class="inline-block {snipView ? 'bg-white' : 'bg-gray-300'} cursor-pointer
    rounded-full h-6 w-6 border-2 border-gray-400">
    <div class="triangle {snipView ? 'down': 'up'}"></div>
  </div>
</div>
<small class="{snipView ? 'hidden': 'block'} text-xxs text-green-500"><img class="h-3 text-green-600 inline-block"
    src="tick-inside-circle.svg" /> This vendor is mapped</small>
<div class="pt-5"></div>
<div class="{snipView ? 'flex': 'hidden'} justify-between items-baseline text-xs">
  <div>00003526</div>
  <div>July 09, 2017</div>
  <div>Montys' Cheese Shop</div>
  <div class="text-gray-600 text-xxs w-20 truncate">Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum</div>
  <div class="flex items-baseline">
    <div class="text-gray-600 text-xxxs">TOTAL</div>
    <div class="text-lg">$10,0000.00</div>
  </div>
</div>
<div class="{snipView ? 'hidden': 'block'}">
  <div class="flex justify-between items-center">
    <div class="py-3 w-40 h-16 flex flex-col justify-around border-t border-b">
      <div class="text-xxs text-gray-600 uppercase pb-2">Invoice</div>
      <div class="text-xs">00003526</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around border-t border-b">
      <div class="text-xxs text-gray-600 uppercase pb-2">Invoice Type</div>
      <div class="text-xs">Receipt</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around border-t border-b">
      <div class="text-xxs text-gray-600 uppercase pb-2">Restaurant</div>
      <div class="text-xs">Monty's Cheese Shop</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around border-t border-b">
      <div class=" flex flex-col justify-center">
        <div class=" flex justify-between items-baseline">
          <div class="text-xxxs text-gray-500 uppercase pb-2">Sub Total</div>
          <div class="text-xxs text-gray-600">$1300.00</div>
        </div>
        <div class="flex justify-between items-baseline">
          <div class="text-xxxs text-gray-500 uppercase">Tax</div>
          <div class="text-xxs text-gray-600">$26.32.00</div>
        </div>
      </div>
    </div>
  </div>

  <div class="flex justify-between items-center">
    <div class="py-3 w-40 h-16 flex flex-col justify-around">
      <div class="text-xxxs text-gray-500 uppercase pb-2">Posting Date</div>
      <div class="text-xs">07 July 2017</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around">
      <div class="text-xxxs text-gray-500 uppercase pb-2">Invoice Date</div>
      <div class="text-xs">July 14, 2017</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around">
      <div class="text-xxxs text-gray-500 uppercase pb-2">Due Date</div>
      <div class="text-xs">Sep 09, 2017</div>
    </div>
    <div class="py-3 w-40 h-16 flex flex-col justify-around">
      <div class="py-2 flex justify-between items-baseline">
        <div class="text-xxxs text-gray-500 uppercase pb-2">Total</div>
        <div class="text-xxs text-gray-600">$10,000</div>
      </div>
    </div>
  </div>

  <div class="border-t w-1/2 text-xxs text-gray-500 pt-4">
    Click to enter Memo
  </div>

</div>