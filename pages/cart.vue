<template>
  <div>
    <div class="bg-[url('/menu-page.jpg')] px-20">
      <div id="menu" class="grid grid-cols-2 py-5">
        <div id="menu-left">
          <img src="/logo.png" class="w-[150px]" alt="" />
        </div>
        <div id="menu-right">
          <ul class="grid grid-cols-5 text-lg font-oswald text-white uppercase pt-5">
            <li>About Us</li>
            <NuxtLink to="/menu">Our Menu</NuxtLink>
            <li>Location</li>
            <li>Contacts</li>
            <NuxtLink to="/cart">Cart</NuxtLink>
          </ul>
        </div>
      </div>
      <h1 class="text-white font-oswald uppercase text-6xl text-center pt-24 pb-28">
        Shopping Cart
      </h1>
    </div>

    <table class="table-auto w-2/3 mt-20 mx-auto">
      <thead>
        <tr>
          <th class="text-left">Name</th>
          <th class="text-right">Price</th>
          <th>Quantity</th>
          <th class="text-right">Total</th>
          <th>Remove</th>
        </tr>
      </thead>
      <tbody>
        <tr
          v-for="order in $store.state.orders"
          :key="order.name"
          class="font-oswald uppercase text-2xl border-b"
        >
          <td class="py-10">{{ order.name }}</td>
          <td class="text-right">RM {{ order.price }}</td>
          <td class="text-center">{{ order.quantity }}</td>
          <td class="text-right">RM {{ order.price * order.quantity }}</td>
          <td class="text-center"><button>✖️</button></td>
        </tr>
      </tbody>
    </table>
  </div>
</template>
