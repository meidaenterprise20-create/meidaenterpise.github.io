import React from 'react';
import Head from 'next/head';
import { 
  Beaker, 
  Truck, 
  Factory, 
  CheckCircle2, 
  Phone, 
  MapPin, 
  ShieldCheck, 
  Clock, 
  BadgeDollarSign,
  ArrowRight
} from 'lucide-react';

// --- Data --- //

const products = [
  { bn: 'সফটনার', en: 'Softener' },
  { bn: 'লিকুইড ডিটারজেন্ট', en: 'Liquid Detergent' },
  { bn: 'কালার কারেক্টর এজেন্ট', en: 'Color Corrector Agent' },
  { bn: 'ব্লিচ লিকুইড', en: 'Bleach Liquid' },
  { bn: 'অয়েল রিমুভিং এজেন্ট', en: 'Oil Removing Agent' },
  { bn: 'কালার ফিক্সিং এজেন্ট', en: 'Color Fixing Agent' },
  { bn: 'সলিউবল কাটিং অয়েল', en: 'Soluble Cutting Oil' },
  { bn: 'কাটিং কম্পাউন্ড', en: 'Cutting Compound' },
  { bn: 'সিলিকন ইমলশন', en: 'Silicone Emulsion' },
  { bn: 'ডিসইনফেকটেন্ট লিকুইড', en: 'Disinfectant Liquid' },
  { bn: 'স্যানিটাইজার লিকুইড', en: 'Sanitizer Liquid' },
  { bn: 'অ্যান্টি রাস্ট অয়েল', en: 'Anti-Rust Oil' },
  { bn: 'ওয়াটার বেসড রিলিজ এজেন্ট', en: 'Water-based Release Agent' },
  { bn: 'অয়েল বেসড রিলিজ এজেন্ট', en: 'Oil-based Release Agent' },
];

const features = [
  {
    icon: <Factory className="w-6 h-6 text-blue-600" />,
    bn: 'সকল পণ্য চায়না থেকে আমদানিকৃত',
    en: 'All products imported from China'
  },
  {
    icon: <Truck className="w-6 h-6 text-blue-600" />,
    bn: 'গার্মেন্টস ও ফ্যাক্টরির জন্য বাল্ক সরবরাহ',
    en: 'Bulk supply for garments & factories'
  },
  {
    icon: <CheckCircle2 className="w-6 h-6 text-blue-600" />,
    bn: 'দ্রুত ডেলিভারি ও নির্ভরযোগ্য মান',
    en: 'Fast delivery & reliable quality'
  }
];

const benefits = [
  {
    icon: <Clock className="w-10 h-10 text-white" />,
    title: 'Fast Delivery',
    desc: 'দ্রুত ডেলিভারি'
  },
  {
    icon: <ShieldCheck className="w-10 h-10 text-white" />,
    title: 'Reliable Quality',
    desc: 'নির্ভরযোগ্য মান'
  },
  {
    icon: <BadgeDollarSign className="w-10 h-10 text-white" />,
    title: 'Best Price',
    desc: 'সেরা মূল্য'
  }
];

// --- Components --- //

export default function MeidaEnterprise() {
  const scrollToContact = () => {
    document.getElementById('contact-section')?.scrollIntoView({ behavior: 'smooth' });
  };

  return (
    <div className="min-h-screen bg-slate-50 font-sans text-slate-800">
      <Head>
        <title>Meida Enterprise - Industrial & Household Chemicals</title>
        <meta name="description" content="Meida Enterprise: High-quality industrial and household chemicals in Bangladesh. Bulk supply for factories." />
      </Head>

      {/* Navigation */}
      <nav className="bg-white border-b border-slate-200 sticky top-0 z-50">
        <div className="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="flex justify-between h-16 items-center">
            <div className="flex items-center gap-2">
              <div className="bg-blue-600 p-1.5 rounded-lg">
                <Beaker className="w-6 h-6 text-white" />
              </div>
              <span className="font-bold text-xl text-slate-900 tracking-tight">
                Meida Enterprise
              </span>
            </div>
            <div className="hidden md:flex items-center gap-6 font-medium text-sm">
              <a href="#about" className="text-slate-600 hover:text-blue-600 transition">About</a>
              <a href="#products" className="text-slate-600 hover:text-blue-600 transition">Products</a>
              <button 
                onClick={scrollToContact}
                className="bg-blue-600 text-white px-4 py-2 rounded-md hover:bg-blue-700 transition flex items-center gap-2"
              >
                <Phone className="w-4 h-4" />
                Contact Us
              </button>
            </div>
          </div>
        </div>
      </nav>

      {/* Hero Section */}
      <header className="relative bg-slate-900 overflow-hidden">
        <div className="absolute inset-0 bg-gradient-to-br from-blue-900 to-slate-900 opacity-90" />
        {/* Decorative blurry blobs */}
        <div className="absolute -top-24 -left-24 w-96 h-96 bg-blue-600 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob" />
        <div className="absolute top-32 -right-24 w-96 h-96 bg-cyan-500 rounded-full mix-blend-multiply filter blur-3xl opacity-20 animate-blob animation-delay-2000" />
        
        <div className="relative max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 py-24 md:py-32">
          <div className="max-w-3xl">
            <h1 className="text-4xl md:text-5xl lg:text-6xl font-extrabold text-white tracking-tight mb-6 leading-tight">
              <span className="block text-blue-400 mb-2 text-2xl md:text-3xl font-bold uppercase tracking-widest">Quality Chemicals</span>
              ইন্ডাস্ট্রিয়াল ও হাউজহোল্ড কেমিক্যাল সরবরাহকারী
            </h1>
            <p className="text-lg md:text-xl text-slate-300 mb-8 max-w-2xl">
              Trusted supplier of Industrial & Household Chemicals in Bangladesh. 
            </p>
            <div className="flex flex-col sm:flex-row gap-4">
              <button 
                onClick={scrollToContact}
                className="inline-flex items-center justify-center px-6 py-3.5 border border-transparent text-base font-medium rounded-md text-white bg-blue-600 hover:bg-blue-700 transition shadow-lg hover:shadow-blue-500/25"
              >
                অর্ডার করুন (Order Now)
                <ArrowRight className="ml-2 w-5 h-5" />
              </button>
              <a 
                href="#products"
                className="inline-flex items-center justify-center px-6 py-3.5 border-2 border-slate-600 text-base font-medium rounded-md text-slate-300 hover:text-white hover:border-white transition"
              >
                আমাদের পণ্য দেখুন
              </a>
            </div>
          </div>
        </div>
      </header>

      {/* Introduction & Key Points */}
      <section id="about" className="py-16 md:py-24 bg-white">
        <div className="max-w-4xl mx-auto px-4 sm:px-6 lg:px-8 text-center mb-12">
          <span className="inline-block px-3 py-1 text-sm font-semibold text-blue-800 bg-blue-100 rounded-full mb-4">
            About Us
          </span>
          <h2 className="text-3xl font-bold text-slate-900 mb-8">
            Meida Enterprise-এ স্বাগতম
          </h2>
          <div className="bg-slate-50 border border-slate-100 rounded-2xl p-6 md:p-8 shadow-sm text-left md:text-center space-y-6">
            <div className="space-y-4">
              <p className="text-lg md:text-xl text-slate-800 leading-relaxed font-medium">
                "হ্যালো! আমরা Meida Enterprise – বহু বছর ধরে আমরা গুণগতমানসম্পন্ন ইন্ডাস্ট্রিয়াল ও হাউজহোল্ড কেমিক্যাল অফলাইনে বিক্রি করে আসছি, আর এখন আমরা আমাদের ব্যবসা অনলাইনে শুরু করেছি!"
              </p>
              <p className="text-slate-600">
                "Hello! We are Meida Enterprise – for many years we have been selling quality industrial and household chemicals offline, and now we have started our business online!"
              </p>
            </div>
            <div className="pt-4 border-t border-slate-200">
              <p className="text-amber-700 font-medium flex items-center justify-center gap-2 bg-amber-50 p-3 rounded-lg">
                <span className="text-xl">⚠️</span>
                <span>
                  দয়া করে লক্ষ্য করুন: আমাদের তালিকাভুক্ত পণ্যের বাইরে অন্য কোনো পণ্য আমাদের কাছে নেই।
                  <br/>
                  <span className="text-sm font-normal text-amber-800/80">
                  (Please note: We do not possess any products other than those listed.)
                  </span>
                </span>
              </p>
            </div>
          </div>
        </div>

        {/* Key Features Cards */}
        <div className="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid md:grid-cols-3 gap-6">
            {features.map((feature, idx) => (
              <div key={idx} className="bg-white p-6 rounded-xl border border-slate-200 shadow-sm hover:shadow-md transition flex items-start gap-4">
                <div className="bg-blue-50 p-3 rounded-lg shrink-0">
                  {feature.icon}
                </div>
                <div>
                  <h3 className="text-lg font-semibold text-slate-900 mb-1">{feature.bn}</h3>
                  <p className="text-slate-500 text-sm">{feature.en}</p>
                </div>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Product Grid */}
      <section id="products" className="py-16 md:py-24 bg-slate-50">
        <div className="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="text-center mb-12">
            <span className="inline-block px-3 py-1 text-sm font-semibold text-blue-800 bg-blue-100 rounded-full mb-4">
              Our Catalogue
            </span>
            <h2 className="text-3xl md:text-4xl font-bold text-slate-900">
              আমাদের পণ্যসমূহ (Products)
            </h2>
            <p className="mt-4 text-lg text-slate-600 max-w-2xl mx-auto">
              High-quality chemicals for industrial and household use.
            </p>
          </div>

          <div className="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-6">
            {products.map((product, idx) => (
              <div key={idx} className="group bg-white rounded-2xl p-6 shadow-sm border border-slate-200 hover:shadow-md hover:border-blue-300 transition-all duration-300 flex flex-col items-center text-center">
                <div className="mb-4 p-4 bg-slate-100 text-slate-400 rounded-full group-hover:bg-blue-50 group-hover:text-blue-500 transition-colors">
                   <Beaker className="w-8 h-8" />
                </div>
                <h3 className="text-xl font-bold text-slate-800 mb-1">
                  {product.bn}
                </h3>
                <p className="text-slate-500 font-medium">
                  {product.en}
                </p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Benefits Banner */}
      <section className="py-12 bg-blue-600">
        <div className="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid md:grid-cols-3 gap-8 text-center">
            {benefits.map((benefit, idx) => (
              <div key={idx} className="flex flex-col items-center">
                <div className="mb-4 p-3 bg-blue-500/50 rounded-full">
                  {benefit.icon}
                </div>
                <h3 className="text-white text-xl font-bold uppercase tracking-wide">{benefit.title}</h3>
                <p className="text-blue-100 mt-1">{benefit.desc}</p>
              </div>
            ))}
          </div>
        </div>
      </section>

      {/* Contact Section / Footer */}
      <footer id="contact-section" className="bg-slate-900 text-slate-300 py-16">
        <div className="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
          <div className="grid md:grid-cols-2 gap-12">
            {/* Call to Action */}
            <div>
              <h2 className="text-3xl font-bold text-white mb-6">
                অর্ডার করতে যোগাযোগ করুন
                <span className="block text-blue-400 text-2xl mt-2">Contact Us to Order</span>
              </h2>
              <p className="text-lg mb-8 text-slate-400">
                গার্মেন্টস, ফ্যাক্টরি বা ব্যক্তিগত ব্যবহারের জন্য বাল্ক কেমিক্যাল প্রয়োজন? আমরা আছি আপনার পাশে।
                <br/>
                <span className="text-sm">(Need bulk chemicals for garments, factories or personal use? We are here for you.)</span>
              </p>
              
              <div className="space-y-6">
                <a 
                  href="tel:+8801784768183" 
                  className="flex items-center p-4 bg-slate-800/50 rounded-xl border border-slate-700 hover:bg-slate-800 hover:border-blue-500 transition group"
                >
                  <div className="bg-blue-600 p-3 rounded-lg mr-4 group-hover:scale-110 transition-transform">
                    <Phone className="w-6 h-6 text-white" />
                  </div>
                  <div>
                    <p className="text-sm text-slate-400 uppercase font-semibold tracking-wider">Call Us Now</p>
                    <p className="text-2xl font-bold text-white font-mono">01784 768183</p>
                  </div>
                </a>

                <div className="flex items-center p-4 bg-slate-800/50 rounded-xl border border-slate-700">
                  <div className="bg-slate-700 p-3 rounded-lg mr-4">
                    <MapPin className="w-6 h-6 text-slate-300" />
                  </div>
                  <div>
                    <p className="text-sm text-slate-400 uppercase font-semibold tracking-wider">Location</p>
                    <p className="text-xl font-medium text-white">নতুন বাজার, ঢাকা (Notun Bazar, Dhaka)</p>
                  </div>
                </div>
              </div>
            </div>

            {/* Quick Links / Info */}
            <div className="md:pl-12 md:border-l border-slate-800 flex flex-col justify-between">
              <div>
                 <div className="flex items-center gap-2 mb-6">
                  <div className="bg-blue-600 p-1.5 rounded-lg">
                    <Beaker className="w-6 h-6 text-white" />
                  </div>
                  <span className="font-bold text-2xl text-white tracking-tight">
                    Meida Enterprise
                  </span>
                </div>
                <p className="text-slate-400 mb-6">
                  Your reliable partner for high-quality industrial chemicals in Bangladesh.
                </p>
              </div>
              
              <div className="mt-8 pt-8 border-t border-slate-800 text-sm text-slate-500">
                © {new Date().getFullYear()} Meida Enterprise. All rights reserved.
              </div>
            </div>
          </div>
        </div>
      </footer>
    </div>
  );
}
