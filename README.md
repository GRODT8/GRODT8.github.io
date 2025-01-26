import React from "react";
import { motion } from "framer-motion";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { ShoppingCart } from "lucide-react";

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

export default function GRODTShop() {
  return (
    <div className="min-h-screen bg-gray-50 p-4">
      {/* Header */}
      <header className="flex justify-between items-center py-4 px-8 bg-black text-white">
        <h1 className="text-3xl font-bold">GRODT</h1>
        <Button className="flex items-center gap-2 bg-white text-black">
          <ShoppingCart size={18} /> Winkelwagen
        </Button>
      </header>

      {/* Hero Section */}
      <section className="relative bg-black text-white text-center py-16">
        <motion.div
          className="container mx-auto px-4"
          initial={{ opacity: 0, y: 50 }}
          animate={{ opacity: 1, y: 0 }}
          transition={{ duration: 1 }}
        >
          <h2 className="text-4xl font-bold">Get Rich Or Die Trying</h2>
          <p className="text-lg mt-4">Streetwear met een boodschap</p>
          <Button className="mt-6 bg-white text-black">Shop Nu</Button>
        </motion.div>
      </section>

      {/* Product Section */}
      <section className="py-12">
        <h2 className="text-2xl font-bold text-center mb-6">Onze Collectie</h2>
        <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-6 container mx-auto px-4">
          {products.map((product) => (
            <Card key={product.id} className="hover:shadow-lg">
              <img
                src={product.image}
                alt={product.name}
                className="w-full h-60 object-cover rounded-t-lg"
              />
              <CardContent className="p-4 text-center">
                <h3 className="font-semibold text-lg">{product.name}</h3>
                <p className="text-gray-700">{product.price}</p>
                <Button className="mt-4 bg-black text-white">In Winkelwagen</Button>
              </CardContent>
            </Card>
          ))}
        </div>
      </section>

      {/* Footer */}
      <footer className="bg-black text-white py-6 text-center">
        <p>&copy; 2025 GRODT. Alle rechten voorbehouden.</p>
      </footer>
    </div>
  );
}
