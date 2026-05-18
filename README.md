export default function CryptoTradingWebsite() {
  return (
    <div className="min-h-screen bg-black text-white font-sans">

      {/* Header */}
      <header className="flex items-center justify-between p-6 border-b border-gray-800">
        <h1 className="text-2xl font-bold text-yellow-400">
          CryptoSignal LK
        </h1>

        <nav className="flex gap-6 text-sm">
          <a href="#videos" className="hover:text-yellow-400">
            Videos
          </a>

          <a href="#patterns" className="hover:text-yellow-400">
            Patterns
          </a>

          <a href="#pdf" className="hover:text-yellow-400">
            PDF Notes
          </a>

          <a href="#login" className="hover:text-yellow-400">
            Login
          </a>
        </nav>
      </header>

      {/* Hero Section */}
      <section className="text-center py-24 px-6 bg-gradient-to-b from-gray-900 to-black">
        <h2 className="text-5xl font-bold mb-6 text-yellow-400">
          Learn Binance & Forex Trading
        </h2>

        <p className="text-gray-300 max-w-2xl mx-auto text-lg mb-8">
          Watch trading videos, learn chart patterns, download PDF guides,
          and improve your trading skills.
        </p>

        <div className="flex justify-center gap-4">
          <button className="bg-yellow-400 text-black px-6 py-3 rounded-2xl font-semibold hover:scale-105 transition">
            Join Now
          </button>

          <button className="border border-yellow-400 px-6 py-3 rounded-2xl hover:bg-yellow-400 hover:text-black transition">
            Watch Videos
          </button>
        </div>
      </section>

      {/* Videos */}
      <section id="videos" className="py-16 px-6">
        <h3 className="text-3xl font-bold mb-8 text-yellow-400">
          Trading Videos
        </h3>

        <div className="grid md:grid-cols-3 gap-6">
          {[1, 2, 3].map((item) => (
            <div
              key={item}
              className="bg-gray-900 rounded-3xl p-4 shadow-lg"
            >
              <div className="bg-gray-800 h-48 rounded-2xl mb-4 flex items-center justify-center text-gray-400">
                Video Preview
              </div>

              <h4 className="text-xl font-semibold mb-2">
                Binance Tutorial {item}
              </h4>

              <p className="text-gray-400 text-sm">
                Learn market analysis and smart trading methods.
              </p>
            </div>
          ))}
        </div>
      </section>

      {/* Chart Patterns */}
      <section id="patterns" className="py-16 px-6 bg-gray-950">
        <h3 className="text-3xl font-bold mb-8 text-yellow-400">
          Chart Patterns
        </h3>

        <div className="grid md:grid-cols-4 gap-6">
          {[
            "Head & Shoulders",
            "Double Top",
            "Triangle Pattern",
            "Support & Resistance",
          ].map((pattern) => (
            <div
              key={pattern}
              className="bg-gray-900 p-6 rounded-3xl text-center"
            >
              <div className="text-5xl mb-4">📈</div>

              <h4 className="font-semibold text-lg">
                {pattern}
              </h4>
            </div>
          ))}
        </div>
      </section>

      {/* PDF Section */}
      <section id="pdf" className="py-16 px-6">
        <h3 className="text-3xl font-bold mb-8 text-yellow-400">
          PDF Trading Notes
        </h3>

        <div className="grid md:grid-cols-3 gap-6">
          {[1, 2, 3].map((item) => (
            <div
              key={item}
              className="bg-gray-900 rounded-3xl p-6"
            >
              <div className="text-5xl mb-4">📘</div>

              <h4 className="text-xl font-semibold mb-2">
                Trading Guide {item}
              </h4>

              <button className="mt-4 bg-yellow-400 text-black px-4 py-2 rounded-xl font-semibold">
                Download PDF
              </button>
            </div>
          ))}
        </div>
      </section>

      {/* Login Section */}
      <section id="login" className="py-16 px-6 bg-gray-950">
        <div className="max-w-md mx-auto bg-gray-900 p-8 rounded-3xl shadow-lg">
          <h3 className="text-3xl font-bold mb-6 text-center text-yellow-400">
            Member Login
          </h3>

          <div className="space-y-4">
            <input
              type="email"
              placeholder="Email"
              className="w-full p-3 rounded-xl bg-gray-800 border border-gray-700"
            />

            <input
              type="password"
              placeholder="Password"
              className="w-full p-3 rounded-xl bg-gray-800 border border-gray-700"
            />

            <button className="w-full bg-yellow-400 text-black py-3 rounded-xl font-bold hover:scale-105 transition">
              Login
            </button>
          </div>
        </div>
      </section>

      {/* Footer */}
      <footer className="text-center py-8 border-t border-gray-800 text-gray-500">
        © 2026 CryptoSignal LK — All Rights Reserved.
      </footer>

    </div>
  );
}
