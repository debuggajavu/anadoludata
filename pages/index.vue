<!-- pages/index.vue -->
<template>
  <div>
    <!-- Hero Bölümü -->
    <div id="anasayfa" class="bg-gradient-to-b from-anadolu-beige/10 to-anadolu-teal/5 py-20">
      <div class="container mx-auto px-4">
        <div ref="hero" class="flex flex-col md:flex-row items-center justify-between gap-12">
          <div class="md:w-1/2 space-y-6">
            <h1 class="text-4xl md:text-6xl font-bold tracking-tight">
              AnadoluData <span class="text-anadolu-teal">Çözümleri</span>
            </h1>
            <p class="text-xl text-anadolu-navy/80 max-w-lg">
              Mobil, web, blockchain ve CRM çözümleriyle işletmenizi geleceğe taşıyoruz.
            </p>
            <div class="flex flex-wrap gap-4">
              <Button size="lg" class="px-8 bg-anadolu-teal hover:bg-anadolu-teal/90" @click="kaydirSectionIcin('hizmetler')">Keşfet</Button>
              <Button size="lg" variant="outline" class="px-8 text-anadolu-teal border-anadolu-teal hover:bg-anadolu-teal/10" @click="kaydirSectionIcin('iletisim')">İletişim</Button>
            </div>
          </div>
          <div class="md:w-1/2">
            <div class="w-full h-auto relative bg-white/50 rounded-lg shadow-xl overflow-hidden">
              <img 
                src="/images/herotech.webp" 
                alt="AnadoluData Teknoloji" 
                class="w-full h-auto"
                loading="eager"
                fetchpriority="high">
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Özellikler Bölümü -->
    <div id="hizmetler" class="py-20 bg-white">
      <div class="container mx-auto px-4">
        <div ref="features" class="text-center mb-16">
          <h2 class="text-3xl font-bold mb-4">Dijital Dönüşüm Hizmetlerimiz</h2>
          <p class="text-xl text-gray-600 max-w-2xl mx-auto">
            Modern teknolojilerle özel çözümler geliştiriyoruz
          </p>
        </div>

        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <!-- Web Çözümleri Kartı -->
          <Card class="shadow-md hover:shadow-xl transition-all duration-300 overflow-hidden group hover:scale-105">
            <div class="relative h-48 overflow-hidden">
              <img src="/images/icons/social/website1.webp" alt="Web Çözümleri" 
                  class="w-full h-full object-cover transition-opacity duration-300 group-hover:opacity-0">
              <img src="/images/icons/social/website2.webp" alt="Web Çözümleri" 
                  class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <CardHeader>
              <CardTitle>Web Çözümleri</CardTitle>
            </CardHeader>
            <CardContent>
              <p>Modern ve hızlı web uygulamaları, e-ticaret sistemleri ve kurumsal web siteleri geliştiriyoruz.</p>
            </CardContent>
          </Card>

          <!-- Mobil Uygulamalar Kartı -->
          <Card class="shadow-md hover:shadow-xl transition-all duration-300 overflow-hidden group hover:scale-105">
            <div class="relative h-48 overflow-hidden">
              <img src="/images/icons/social/mobile1.webp" alt="Mobil Uygulamalar" 
                  class="w-full h-full object-cover transition-opacity duration-300 group-hover:opacity-0">
              <img src="/images/icons/social/mobile2.webp" alt="Mobil Uygulamalar" 
                  class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <CardHeader>
              <CardTitle>Mobil Uygulamalar</CardTitle>
            </CardHeader>
            <CardContent>
              <p>iOS ve Android için native performansta, kullanıcı dostu mobil uygulamalar tasarlıyoruz.</p>
            </CardContent>
          </Card>

          <!-- Blockchain Kartı -->
          <Card class="shadow-md hover:shadow-xl transition-all duration-300 overflow-hidden group hover:scale-105">
            <div class="relative h-48 overflow-hidden">
              <img src="/images/icons/social/blockchain1.webp" alt="Blockchain Teknolojileri" 
                  class="w-full h-full object-cover transition-opacity duration-300 group-hover:opacity-0">
              <img src="/images/icons/social/blockchain2.webp" alt="Blockchain Teknolojileri" 
                  class="absolute inset-0 w-full h-full object-cover opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <CardHeader>
              <CardTitle>Blockchain Teknolojileri</CardTitle>
            </CardHeader>
            <CardContent>
              <p>Güvenli ve şeffaf blockchain tabanlı çözümlerle işletmenizi geleceğe hazırlıyoruz.</p>
            </CardContent>
          </Card>
        </div>
      </div>
    </div>

    <!-- Teknolojiler Bölümü -->
    <div id="teknolojiler" class="py-16 bg-gray-50">
      <div class="container mx-auto px-4">
        <div ref="tech" class="text-center mb-12">
          <h2 class="text-3xl font-bold mb-4">Kullandığımız Teknolojiler</h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            En son teknolojileri kullanarak projelerinizi hayata geçiriyoruz
          </p>
        </div>

        <div class="grid grid-cols-2 sm:grid-cols-3 md:grid-cols-6 gap-8">
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/vue.svg" alt="Vue" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">Vue.js</span>
          </div>
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/react.svg" alt="React" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">React</span>
          </div>
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/node_js.svg" alt="Node.js" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">Node.js</span>
          </div>
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/android.svg" alt="Android" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">Android</span>
          </div>
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/ios.svg" alt="iOS" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">iOS</span>
          </div>
          <div class="flex flex-col items-center">
            <img src="/images/icons/social/figma.svg" alt="Figma" class="w-16 h-16 mb-2">
            <span class="text-sm font-medium">Figma</span>
          </div>
        </div>
      </div>
    </div>

    <!-- Hakkımızda Bölümü -->
    <div id="hakkimizda" class="py-20 bg-white">
      <div class="container mx-auto px-4">
        <div ref="about" class="flex flex-col md:flex-row items-center gap-12">
          <div class="md:w-1/2">
            <div class="w-full h-auto rounded-lg shadow-xl overflow-hidden">
              <img src="/images/team.svg" alt="AnadoluData Ekibi" class="w-full h-auto">
            </div>
          </div>
          <div class="md:w-1/2 space-y-6">
            <h2 class="text-3xl font-bold">Vizyonumuz</h2>
            <p class="text-lg text-gray-600">
              Anadolu'nun teknoloji potansiyelini dünyaya taşıyoruz. İşletmelerin dijital dönüşümüne öncülük ederek, 
              yenilikçi çözümlerle müşterilerimizin başarılarına katkıda bulunuyoruz.
            </p>
            <Button variant="outline" class="border-anadolu-teal text-anadolu-teal hover:bg-anadolu-teal/10" @click="teklifModalAcik = true">Teklif Al</Button>
          </div>
        </div>
      </div>
    </div>

    <!-- İletişim Bölümü -->
    <div id="iletisim" class="py-20 bg-gray-50">
      <div class="container mx-auto px-4">
        <div ref="contact" class="text-center mb-12">
          <h2 class="text-3xl font-bold mb-4">Bize Ulaşın</h2>
          <p class="text-lg text-gray-600 max-w-2xl mx-auto">
            Projeleriniz için bizimle iletişime geçin
          </p>
        </div>
        
        <div class="max-w-lg mx-auto">
          <Card>
            <CardContent class="pt-6">
              <form class="space-y-4" @submit.prevent="gonderFormu">
                <div class="grid grid-cols-2 gap-4">
                  <div class="space-y-2">
                    <label class="text-sm font-medium">Ad <span class="text-red-500">*</span></label>
                    <input 
                      type="text" 
                      class="w-full p-2 border rounded" 
                      v-model="formData.ad"
                      maxlength="50"
                      required 
                    />
                  </div>
                  <div class="space-y-2">
                    <label class="text-sm font-medium">Soyad <span class="text-red-500">*</span></label>
                    <input 
                      type="text" 
                      class="w-full p-2 border rounded" 
                      v-model="formData.soyad"
                      maxlength="50"
                      required 
                    />
                  </div>
                </div>
                <div class="space-y-2">
                  <label class="text-sm font-medium">E-posta <span class="text-red-500">*</span></label>
                  <input 
                    type="email" 
                    class="w-full p-2 border rounded" 
                    v-model="formData.email"
                    maxlength="100"
                    required 
                  />
                </div>
                <div class="space-y-2">
                  <label class="text-sm font-medium">Telefon</label>
                  <input 
                    type="tel" 
                    class="w-full p-2 border rounded" 
                    v-model="formData.telefon"
                    maxlength="20"
                  />
                </div>
                <div class="space-y-2">
                  <label class="text-sm font-medium">Mesaj <span class="text-red-500">*</span></label>
                  <textarea 
                    rows="4" 
                    class="w-full p-2 border rounded"
                    v-model="formData.mesaj"
                    maxlength="300"
                    required
                  ></textarea>
                  <div class="text-xs text-gray-500 flex justify-between">
                    <span>Kalan karakter: {{ 300 - formData.mesaj.length }}</span>
                    <span>Maksimum 300 karakter</span>
                  </div>
                </div>
                <Button 
                  class="w-full bg-anadolu-teal hover:bg-anadolu-teal/90 text-white"
                  type="submit" 
                  :disabled="formGonderiliyor"
                >
                  {{ formGonderiliyor ? 'Gönderiliyor...' : 'Gönder' }}
                </Button>

                <!-- Form gönderim durumu -->
                <div v-if="formDurumu" class="mt-4 p-3 rounded" :class="formDurumu.basarili ? 'bg-green-100 text-green-800' : 'bg-red-100 text-red-800'">
                  {{ formDurumu.mesaj }}
                </div>
              </form>
            </CardContent>
          </Card>
        </div>
      </div>
    </div>

    <!-- Footer -->
    <footer class="bg-anadolu-navy text-white py-12">
      <div class="container mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
          <div>
  <div class="flex items-center gap-2 mb-4">
    <img src="/images/logo.svg" alt="AnadoluData Logo" class="h-8 w-auto">
    <h3 class="text-xl font-bold text-anadolu-beige">AnadoluData</h3>
  </div>
  <p class="text-gray-300">Modern teknoloji ve bütçe dostu çözümler</p>
</div>
          <div>
            <h4 class="font-bold mb-4 text-anadolu-beige">Hizmetler</h4>
            <ul class="space-y-2">
              <li>Web Geliştirme</li>
              <li>Mobil Uygulamalar</li>
              <li>Blockchain</li>
              <li>CRM Çözümleri</li>
            </ul>
          </div>
          <div>
            <h4 class="font-bold mb-4 text-anadolu-beige">İletişim</h4>
            <ul class="space-y-2">
              <li>bilgi@anadoludata.com</li>
              <li>İstanbul, Türkiye</li>
            </ul>
          </div>
        </div>
        <div class="border-t border-anadolu-teal/20 mt-8 pt-8 text-center text-gray-400">
          <p>© 2025 AnadoluData. Tüm hakları saklıdır.</p>
        </div>
      </div>
    </footer>
    
    <!-- Teklif Modal -->
    <TeklifModal v-model="teklifModalAcik" />
  </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'
import { useMotion } from '@vueuse/motion'
import { Button } from '@/components/ui/button'
import { Card, CardHeader, CardTitle, CardContent } from '@/components/ui/card'
import TeklifModal from '@/components/TeklifModal.vue'

const hero = ref(null)
const features = ref(null)
const tech = ref(null)
const about = ref(null)
const contact = ref(null)

const teklifModalAcik = ref(false)

const formData = ref({
  ad: '',
  soyad: '',
  email: '',
  telefon: '',
  mesaj: ''
});

const formGonderiliyor = ref(false);
const formDurumu = ref(null);

const kaydirSectionIcin = (id) => {
  const element = document.getElementById(id);
  if (element) {
    element.scrollIntoView({ behavior: 'smooth' });
  }
};

const gonderFormu = async () => {
  formGonderiliyor.value = true;
  
  try {
    // Sunucuya gönder
    const response = await fetch('http://66.179.240.190:3000/api/iletisim', {
      method: 'POST',
      headers: {
        'Content-Type': 'application/json',
      },
      body: JSON.stringify(formData.value)
    });
    
    if (!response.ok) {
      throw new Error('Sunucu hatası');
    }
    
    // Başarılı gönderim
    formDurumu.value = {
      basarili: true,
      mesaj: 'Mesajınız başarıyla gönderildi. En kısa sürede size dönüş yapacağız.'
    };
    
    // Formu temizle
    formData.value = {
      ad: '',
      soyad: '',
      email: '',
      telefon: '',
      mesaj: ''
    };
  } catch (error) {
    // Hata durumu
    formDurumu.value = {
      basarili: false,
      mesaj: 'Mesaj gönderilirken bir hata oluştu. Lütfen daha sonra tekrar deneyin.'
    };
    console.error('Form gönderim hatası:', error);
  } finally {
    formGonderiliyor.value = false;
  }
};

onMounted(() => {
  useMotion(hero, {
    initial: { opacity: 0, y: 100 },
    enter: { 
      opacity: 1, 
      y: 0,
      transition: { duration: 800 }
    }
  })

  useMotion(features, {
    initial: { opacity: 0, scale: 0.9 },
    enter: { 
      opacity: 1,
      scale: 1,
      transition: { delay: 200, duration: 600 }
    },
    visibleOnce: true
  })

  useMotion(tech, {
    initial: { opacity: 0 },
    enter: { 
      opacity: 1,
      transition: { delay: 300, duration: 800, staggerChildren: 0.1 }
    },
    visibleOnce: true
  })

  useMotion(about, {
    initial: { opacity: 0, x: -50 },
    enter: { 
      opacity: 1,
      x: 0,
      transition: { delay: 200, duration: 800 }
    },
    visibleOnce: true
  })

  useMotion(contact, {
    initial: { opacity: 0, y: 50 },
    enter: { 
      opacity: 1,
      y: 0,
      transition: { delay: 200, duration: 600 }
    },
    visibleOnce: true
  })
})
</script>