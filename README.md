import React from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Truck, Boxes, Search, LogIn, UserPlus, Info } from "lucide-react";

export default function HomePage() {
  return (
    <div className="min-h-screen bg-blue-100 p-4">
      <header className="text-center mb-8">
        <h1 className="text-4xl font-bold text-blue-800">Digital Logistics</h1>
        <p className="text-blue-700">Empowering logistics across Africa and beyond</p>

        <div className="flex justify-center gap-4 mt-4">
          <Button variant="outline" className="flex items-center gap-2">
            <LogIn size={16} /> Login
          </Button>
          <Button className="flex items-center gap-2">
            <UserPlus size={16} /> Register
          </Button>
        </div>
      </header>

      <section className="mb-8 max-w-4xl mx-auto text-center">
        <h2 className="text-2xl font-bold text-blue-800 mb-2">Our Mission</h2>
        <p className="text-gray-700">
          Reframe logistics challenges and bring optimal solutions.
        </p>
      </section>

      <section className="mb-8 max-w-4xl mx-auto text-center">
        <h2 className="text-2xl font-bold text-blue-800 mb-2">Vision</h2>
        <p className="text-gray-700">
          To build a smart, inclusive, and efficient logistics platform that empowers businesses,
          reduces cost, and improves supply chain transparency globally.
        </p>
      </section>

      <section className="mb-8 max-w-4xl mx-auto text-center">
        <h2 className="text-2xl font-bold text-blue-800 mb-2">Core Values</h2>
        <p className="text-gray-700">
          Innovation, Collaboration, Sustainability, Inclusion, and Continuous Learning.
        </p>
      </section>

      <section className="mb-8 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold text-blue-800 mb-2 text-center">Why Digital Logistics?</h2>
        <ul className="text-gray-700 list-disc pl-6">
          <li>✔️ Lower operational costs through automation and real-time tracking</li>
          <li>✔️ Better coordination of inventory, transport, and supply chain data</li>
          <li>✔️ Accessibility from mobile devices, empowering even small businesses</li>
          <li>⚠️ Risk of job displacement — but creates new roles in digital logistics management</li>
        </ul>
      </section>

      <section className="mb-8 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold text-blue-800 mb-2 text-center">Brief History of Logistics</h2>
        <p className="text-gray-700">
          Logistics began in military operations, ensuring troops had supplies where and when
          needed. Over time, it evolved into a core business discipline—covering the movement,
          storage, and flow of goods globally. The digital era has transformed logistics into a
          tech-driven ecosystem.
        </p>
      </section>

      <section className="mb-12 max-w-4xl mx-auto">
        <h2 className="text-2xl font-bold text-blue-800 mb-2 text-center">What Digital Logistics Offers</h2>

        <div className="space-y-4">
          <div>
            <h3 className="text-xl font-semibold text-blue-700">Inventory Management</h3>
            <p className="text-gray-700">
              Track stock levels, warehouse movements, and product availability in real time.
              Reduces overstocking and out-of-stock issues.
            </p>
          </div>

          <div>
            <h3 className="text-xl font-semibold text-blue-700">Transport Coordination</h3>
            <p className="text-gray-700">
              Plan and monitor deliveries, assign transport routes, and improve vehicle utilization.
              Minimizes delivery delays and fuel costs.
            </p>
          </div>

          <div>
            <h3 className="text-xl font-semibold text-blue-700">Supply Chain Visibility</h3>
            <p className="text-gray-700">
              Get insights into your entire supply process—from supplier to final delivery. It
              supports better decision-making and risk management.
            </p>
          </div>
        </div>
      </section>

      <div className="grid gap-6 md:grid-cols-3">
        <Card>
          <CardContent className="flex flex-col items-center p-6">
            <Boxes size={48} className="text-blue-600 mb-2" />
            <h2 className="text-xl font-semibold mb-2">Inventory Tracking</h2>
            <p className="text-center text-sm text-gray-600">
              Monitor stock levels, location, and movement in real-time.
            </p>
            <Button className="mt-4">Go to Inventory</Button>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="flex flex-col items-center p-6">
            <Truck size={48} className="text-blue-600 mb-2" />
            <h2 className="text-xl font-semibold mb-2">Transport Management</h2>
            <p className="text-center text-sm text-gray-600">
              Plan, execute, and optimize transport operations.
            </p>
            <Button className="mt-4">Manage Transport</Button>
          </CardContent>
        </Card>

        <Card>
          <CardContent className="flex flex-col items-center p-6">
            <Search size={48} className="text-blue-600 mb-2" />
            <h2 className="text-xl font-semibold mb-2">Supply Chain Visibility</h2>
            <p className="text-center text-sm text-gray-600">
              Gain insights into the full supply chain for better decisions.
            </p>
            <Button className="mt-4">View Dashboard</Button>
          </CardContent>
        </Card>
      </div>

      <footer className="mt-16 text-center text-sm text-gray-600">
        <div className="flex justify-center items-center gap-2 mb-2">
          <Info size={14} />
          <span>Built by African youth – Dreaming big, working smart.</span>
        </div>
        <p>&copy; {new Date().getFullYear()} Digital Logistics Platform. All rights reserved.</p>
        <p className="mt-2 text-xs">Inspired by AIESEC youth and Aspire Leaders from Niger.</p>
      </footer>
    </div>
  );
}
