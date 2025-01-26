const products = [
  {
    id: 1,
    name: "GRODT Hoodie",
    price: "€59,99",
    image: "https://via.placeholder.com/300x400",
  },
  {
    id: 2,
    name: "GRODT T-Shirt",
    price: "€29,99",
    image: "https://via.placeholder.com/300x400",
  },
  {
    id: 3,
    name: "GRODT Cap",
    price: "€19,99",
    image: "https://via.placeholder.com/300x400",
  },
  {
    id: 4,
    name: "GRODT Joggers",
    price: "€49,99",
    image: "https://via.placeholder.com/300x400",
  },
];

function createProductCard(product) {
  return `
    <div class="card hover:shadow-lg">
      <img
        src="${product.image}"
        alt="${product.name}"
        class="w-full h-60 object-cover rounded-t-lg"
      />
      <div class="p-4 text-center">
        <h3 class="font-semibold text-lg">${product.name}</h3>
        <p class="text-gray-700">${product.price}</p>
        <button class="mt-4 bg-black text-white px-4 py-2 rounded">In Winkelwagen</button>
      </div>
    </div>
  `;
}

function renderProducts() {
  const productsContainer = document.getElementById("products-container");
  productsContainer.innerHTML = products.map(createProductCard).join("");
}

document.addEventListener("DOMContentLoaded", () => {
  renderProducts();
});

// Basic HTML structure for the page
document.body.innerHTML = `
  <div class="min-h-screen bg-gray-50 p-4">
    <!-- Header -->
    <header class="flex justify-between items-center py-4 px-8 bg-black text-white">
      <h1 class="text-3xl font-bold">GRODT</h1>
      <button class="flex items-center gap-2 bg-white text-black px-4 py-2 rounded">
        <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor" stroke-width="2">
          <path stroke-linecap="round" stroke-linejoin="round" d="M3 3h18M3 8h18M7 21h10M12 3v18" />
        </svg>
        Winkelwagen
      </button>
    </header>

    <!-- Hero Section -->
    <section class="relative bg-black text-white text-center py-16">
      <div class="container mx-auto px-4">
        <h2 class="text-4xl font-bold">Get Rich Or Die Trying</h2>
        <p class="text-lg mt-4">Streetwear met een boodschap</p>
        <button class="mt-6 bg-white text-black px-4 py-2 rounded">Shop Nu</button>
      </div>
    </section>

    <!-- Product Section -->
    <section class="py-12">
      <h2 class="text-2xl font-bold text-center mb-6">Onze Collectie</h2>
      <div id="products-container" class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 container mx-auto px-4">
        <!-- Products will be rendered here -->
      </div>
    </section>

    <!-- Footer -->
    <footer class="bg-black text-white py-6 text-center">
      <p>&copy; 2025 GRODT. Alle rechten voorbehouden.</p>
    </footer>
  </div>
`;
