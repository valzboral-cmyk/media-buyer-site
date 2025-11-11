# media-buyer-site
media buyer site
npx create-react-app media-buyer-site
cd media-buyer-site
import React from "react";

// Single-file React component for a media buyer portfolio / lead-gen site.
// Uses Tailwind utility classes. Designed as default export.

export default function MediaBuyerSite() {
  return (
    <div className="min-h-screen bg-gray-50 text-gray-900">
      <header className="max-w-6xl mx-auto p-6 flex items-center justify-between">
        <div className="flex items-center gap-4">
          <div className="w-12 h-12 rounded-lg bg-gradient-to-br from-indigo-600 to-pink-500 flex items-center justify-center text-white font-bold">MB</div>
          <div>
            <h1 className="text-lg font-semibold">Your Name — Media Buyer</h1>
            <p className="text-sm text-gray-500">Performance-focused paid social & programmatic campaigns</p>
          </div>
        </div>
        <nav className="hidden md:flex gap-6 items-center text-sm">
          <a href="#services" className="hover:underline">Services</a>
          <a href="#case-studies" className="hover:underline">Case studies</a>
          <a href="#pricing" className="hover:underline">Pricing</a>
          <a href="#contact" className="btn-outline">Contact</a>
        </nav>
      </header>

      <main className="max-w-6xl mx-auto p-6">
        <section className="grid md:grid-cols-2 gap-8 items-center py-12">
          <div>
            <h2 className="text-4xl font-extrabold leading-tight">Media buying that scales revenue — not just clicks.</h2>
            <p className="mt-4 text-gray-600">I run data-driven paid social, search, and programmatic campaigns for e-commerce and lead gen brands. I focus on creative testing, funnel optimization, and efficient scaling.</p>

            <ul className="mt-6 grid grid-cols-1 sm:grid-cols-2 gap-3">
              <li className="p-3 rounded-lg bg-white shadow-sm">Meta & TikTok Ads</li>
              <li className="p-3 rounded-lg bg-white shadow-sm">Google Ads (Search + YouTube)</li>
              <li className="p-3 rounded-lg bg-white shadow-sm">Programmatic & DV360</li>
              <li className="p-3 rounded-lg bg-white shadow-sm">Analytics & CRO</li>
            </ul>

            <div className="mt-6 flex gap-3">
              <a href="#contact" className="inline-block px-5 py-3 rounded-lg bg-indigo-600 text-white font-semibold">Book a free strategy call</a>
              <a href="#case-studies" className="inline-block px-5 py-3 rounded-lg border border-gray-200">See case studies</a>
            </div>
          </div>

          <div className="p-6 rounded-2xl bg-white shadow-lg">
            <div className="text-sm text-gray-500">Quick contact</div>
            <form className="mt-4 grid gap-3">
              <input className="p-3 border rounded" placeholder="Your name" />
              <input className="p-3 border rounded" placeholder="Email" />
              <input className="p-3 border rounded" placeholder="Website (optional)" />
              <textarea className="p-3 border rounded h-28" placeholder="Tell me about your goal or budget"></textarea>
              <div className="flex gap-3">
                <button type="submit" className="px-4 py-2 rounded bg-indigo-600 text-white">Send</button>
                <a href="mailto:you@yourdomain.com" className="px-4 py-2 rounded border">Email me</a>
              </div>
            </form>
            <div className="mt-4 text-xs text-gray-400">By submitting you agree to be contacted about your inquiry.</div>
          </div>
        </section>

        <section id="services" className="py-12">
          <h3 className="text-2xl font-bold">Services I offer</h3>
          <div className="mt-6 grid md:grid-cols-3 gap-6">
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">Full-funnel media buying</h4>
              <p className="text-sm text-gray-600 mt-2">Strategy, campaign setup, creative testing, optimization, and scaling across channels.</p>
            </div>
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">Creative & CRO playbooks</h4>
              <p className="text-sm text-gray-600 mt-2">Ad creative direction, landing page split tests, and conversion rate improvement.</p>
            </div>
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">Analytics & reporting</h4>
              <p className="text-sm text-gray-600 mt-2">Dashboard set-up, UTM frameworks, and attribution-aware reporting.</p>
            </div>
          </div>
        </section>

        <section id="case-studies" className="py-12">
          <h3 className="text-2xl font-bold">Case studies</h3>
          <div className="mt-6 grid md:grid-cols-2 gap-6">
            <article className="p-6 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">DTC skincare — 3x ROAS scale</h4>
              <p className="text-sm text-gray-600 mt-2">Scaled from $50k to $200k monthly while reducing CAC via creative + funnel changes.</p>
              <div className="mt-3 text-xs text-gray-400">Metrics: ROAS, CAC, LTV uplift</div>
            </article>
            <article className="p-6 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">SaaS lead gen — 40% lower CPL</h4>
              <p className="text-sm text-gray-600 mt-2">Optimized audience flows and ad copy to cut cost-per-lead while increasing demo requests.</p>
              <div className="mt-3 text-xs text-gray-400">Metrics: CPL, qualified lead rate</div>
            </article>
          </div>
        </section>

        <section id="pricing" className="py-12">
          <h3 className="text-2xl font-bold">Pricing models</h3>
          <div className="mt-6 grid md:grid-cols-3 gap-6">
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">Monthly retainer</h4>
              <p className="text-sm text-gray-600 mt-2">Fixed fee for strategy, management & reporting. Best for predictable work.</p>
            </div>
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">% of ad spend</h4>
              <p className="text-sm text-gray-600 mt-2">Aligns incentives — usually combined with a minimum retainer.</p>
            </div>
            <div className="p-5 bg-white rounded-lg shadow-sm">
              <h4 className="font-semibold">Performance bonus</h4>
              <p className="text-sm text-gray-600 mt-2">Bonus based on agreed KPIs (CPA/ROAS/Revenue milestones).</p>
            </div>
          </div>
        </section>

        <section id="contact" className="py-12">
          <h3 className="text-2xl font-bold">Ready to grow?</h3>
          <p className="text-gray-600 mt-2">Book a 30-minute call to walk through your funnel — I’ll bring an audit and quick wins.</p>
          <div className="mt-6">
            <a href="#" className="inline-block px-6 py-3 rounded-lg bg-indigo-600 text-white">Book a call (Calendly link)</a>
            <a href="mailto:you@yourdomain.com" className="ml-4 inline-block px-6 py-3 rounded-lg border">Email me</a>
          </div>
        </section>

        <footer className="mt-12 py-8 text-center text-sm text-gray-500">© {new Date().getFullYear()} Your Name — Media Buyer. Links: Privacy • Terms</footer>
      </main>

      <style jsx>{`
        .btn-outline{ padding: 8px 12px; border-radius: 8px; border: 1px solid rgba(0,0,0,0.06); }
      `}</style>
    </div>
  );
}
npm start
