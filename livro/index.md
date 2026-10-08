---
layout: default
---

<!-- MANIFESTO DO LIVRO (Onde o Dvorak bate) -->
    <article class="bg-zinc-900 text-white py-16 px-6 mt-12 border-t-8 border-brand-red">
        <div class="max-w-4xl mx-auto">
            <h3 class="font-heading text-4xl md:text-5xl font-bold uppercase mb-8 border-b-4 border-white pb-2 inline-block">
                O Livro: <span class="text-brand-red">A Gênese e o Asfalto</span>
            </h3>
            <p class="text-zinc-400 text-xl mb-10">Escrito com sangue, suor e dados. Acompanhe a dissecção do manicômio invisível em tempo real.</p>

            <!-- O Loop do Jekyll -->
            <div class="space-y-6">
              {% for capitulo in site.livro %}
                <div class="bg-brand-dark border-2 border-brand-red p-6 brutalist-btn light-shadow transition-all hover:bg-zinc-800">
                  <a href="{{ capitulo.url }}" class="block">
                    <h4 class="font-heading text-3xl font-black text-white uppercase mb-2">
                        {{ capitulo.title }}
                    </h4>
                    <p class="text-zinc-300 font-medium text-lg">
                        {{ capitulo.excerpt | strip_html | truncatewords: 25 }}...
                    </p>
                    <span class="text-brand-red font-bold uppercase mt-4 block text-sm tracking-widest">
                        Ler Capítulo >_
                    </span>
                  </a>
                </div>
              {% endfor %}
            </div>
        </div>
    </article>

