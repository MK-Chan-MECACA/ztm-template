<template>
  <div>
    <div id="header" class="bg-[url('/hero-bg.jpg')] px-20">
      <div id="menu" class="grid grid-cols-2 py-5">
        <div id="menu-left">
          <img src="logo.png" class="w-[150px]" alt="" />
        </div>
        <div id="menu-right">
          <ul class="grid grid-cols-4 text-lg font-oswald text-white uppercase pt-5">
            <li class="text-ellipsis overflow-hidden">About Us</li>
            <li class="text-ellipsis overflow-hidden">Our Menu</li>
            <li class="text-ellipsis overflow-hidden">Location</li>
            <li class="text-ellipsis overflow-hidden">Contacts</li>
          </ul>
        </div>
      </div>
      <div class="grid grid-cols-2 pb-20 pt-10">
        <img src="hero-burger.png" class="pr-8 mt-10" alt="" />
        <div>
          <h1 class="text-8xl text-white text-center font-lilita font-bold uppercase">
            Classic Burger
          </h1>
          <h2
            class="text-6xl text-white text-center font-lilita font-bold uppercase my-5"
          >
            With Onion
          </h2>
          <p class="text-white font-roboto font-light text-center">
            Our signature burger now comes with onion and cheese. You can customize it to
            your likings. Freshly made to order, all in a Brioche style bun.
          </p>
        </div>
      </div>
    </div>
    <div
      id="section-1"
      class="text-center bg-[url('/about.jpg')] pb-60 bg-cover bg-center"
    >
      <h1 class="text-6xl uppercase font-oswald text-center pt-20 px-24">
        The burger tastes better when you eat it with family
      </h1>
      <p class="font-oswald font-light text-gray-500 text-center text-lg py-6 px-28">
        Spend quality time with your family and eat an affordable, nutritious and
        delicious meal together. Not all burgers are fast foods. All our burgers are
        handmade to orders for you an your family members to enjoy.
      </p>
      <div class="text-center">
        <button class="font-oswald uppercase bg-red-500 text-white py-3 px-8">
          Explore Full Menu
        </button>
      </div>
    </div>
    <div id="section-3" class="text-center">
      <h2 class="text-6xl font-oswald text-red-500 uppercase font-medium pt-20">
        Our Crazy Burgers
      </h2>
      <p class="text-gray-500 font-light text-xl my-10 px-20">
        Whether you are looking for the classics, our specialties, or just wraps, salads,
        and fries. We have it all. We always have something that rewards your tastebuds.
      </p>

      <div class="grid grid-cols-2 px-40 gap-5">
        <div id="left-item-column">
          <Item
            image="crispy-chicken.jpg"
            title="Crispy Chicken"
            description="Chicken breast, chili sauce, tomatoes, pickles, coleslaw"
            price="11.99"
          />
          <Item
            image="baa-baa.jpg"
            title="Baa-Baa Black Sheep"
            description="American cheese, tomato relish, avocado, lettuce, red onion"
            price="15.35"
          />
        </div>
        <div id="right-item-column">
          <Item
            image="ultimate-bacon.jpg"
            title="Ultimate Bacon"
            description="House beef patty, cheddar cheese, smokey bacon, onion, mustard"
            price="14.99"
          />
          <Item
            image="double-burger.jpg"
            title="Double Burger"
            description="2 x beef patties, cheddar cheese, mustard, pickles, tomatoes"
            price="17.99"
          />
        </div>
      </div>
    </div>
  </div>
</template>
