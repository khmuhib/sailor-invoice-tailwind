<template>
  <div class="flex flex-col gap-y-3 py-3">
    <div class="flex justify-between items-center">
      <div class="">
        <h2 class="text-[22px]">Products</h2>
      </div>
      <div class="">
        <button class="bg-[#00C3FF] text-white text-[14px]  py-[7px] px-[20px] rounded-md"><i
            class="fa-solid fa-circle-plus"></i> Add New Product</button>
      </div>
    </div>

    <div class="flex gap-x-3">
      <button class="shadow-sm px-3 py-1 border rounded-md"><i class="fa-solid fa-filter"></i> Filter</button>
      <button class="shadow-sm px-3 py-1 border rounded-md"><i class="fa-solid fa-arrow-up-right-from-square"></i>
        Export</button>
      <button class="shadow-sm px-3 py-1 border rounded-md"><i class="fa-solid fa-upload"></i> Import</button>
    </div>

    <div class="bg-white w-full overflow-hidden rounded-md">
      <table class="w-full overflow-auto overflow-x-scroll">
        <thead class="border-b">
          <tr class="h-[50px]">
            <th class="text-center px-2"><i class="fa-regular fa-circle text-[14px]"></i></th>
            <th class="">Name</th>
            <th class="">Email</th>
            <th class="">Name</th>
            <th class=" text-right pr-3">Action</th>
          </tr>
        </thead>
        <tbody>
          <tr class="h-[50px]">
            <th class="py-2 text-center px-2"><i class="fa-regular fa-circle text-[14px]"></i></th>
            <td>Kh Muhib</td>
            <td>nuhib@gmail.com</td>
            <td>Kh Muhib</td>
            <td class="text-right pr-3"><i class="fa-solid fa-ellipsis"></i></td>
          </tr>
          
        </tbody>
      </table>
    </div>
  </div>






  <p id="demo"></p>

</template>

<script>
export default {
  mounted() {
    document.getElementById("demo").innerHTML = "My First JavaScript";
    const fruits = new Map([
      ["apples", 500],
      ["bananas", 300],
      ["oranges", 200]
    ]);

    document.getElementById("demo").innerHTML = fruits.get("apples");
  }

}
</script>

<style>

</style>