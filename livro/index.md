---
layout: livro
title: "Livro"
date: 2026-10-06
subtitle: "A dor do luto em vida, o colapso dorsal e o isolamento na caixa de pedra."
---

<!-- MANIFESTO DO LIVRO (Onde o Dvorak bate) -->
<article class="bg-zinc-950 text-white py-16 px-5 sm:px-6 mt-12 border-t-4 border-amber-500 selection:bg-amber-500 selection:text-zinc-900">
    <div class="max-w-3xl mx-auto">
        
        <!-- Etiqueta Superior -->
        <div class="font-tech text-amber-500 text-xs tracking-[0.2em] uppercase font-bold mb-4 flex items-center gap-2">
            <span class="w-2 h-2 bg-amber-500 rounded-full animate-pulse"></span>
            Obra Completa
        </div>
        
        <!-- Título -->
        <h3 class="font-ui text-4xl md:text-5xl font-black uppercase mb-8 border-b border-zinc-800 pb-6">
            O Livro: <span class="text-amber-500">A Gênese e o Asfalto</span>
        </h3>
        
        <!-- Manifesto -->
        <p class="font-ui text-zinc-400 text-lg md:text-xl mb-12 leading-relaxed border-l-2 border-amber-500/50 pl-4">
            Escrito com sangue, suor e dados. Acompanhe a dissecção do manicômio invisível em tempo real.
        </p>

        <!-- O Loop do Jekyll -->
        <div class="space-y-6">
            {% for capitulo in site.livro %}
            <div class="bg-black border border-zinc-800 hover:border-amber-500/50 p-6 md:p-8 transition-all group relative overflow-hidden">
                <!-- Efeito Hover (Barra lateral) -->
                <div class="absolute top-0 left-0 w-1 h-full bg-amber-500 opacity-0 group-hover:opacity-100 transition-opacity"></div>
                
                <a href="{{ capitulo.url | relative_url }}" class="block">
                    <!-- Metadados do Capítulo -->
                    <div class="font-tech text-xs text-zinc-500 uppercase tracking-widest mb-3 group-hover:text-amber-400/80 transition-colors">
                        {% if capitulo.date %}
                            {{ capitulo.date | date: "%d/%m/%Y" }} // 
                        {% endif %}
                        Capítulo {{ forloop.index }}
                    </div>
                    
                    <!-- Título do Capítulo -->
                    <h4 class="font-ui text-2xl md:text-3xl font-bold text-zinc-200 group-hover:text-white uppercase tracking-tight mb-3 transition-colors">
                        {{ capitulo.title }}
                    </h4>
                    
                    <!-- Resumo / Subtítulo -->
                    <p class="text-zinc-400 font-medium text-base md:text-lg mb-6">
                        {% if capitulo.subtitle %}
                            {{ capitulo.subtitle }}
                        {% else %}
                            {{ capitulo.excerpt | strip_html | truncatewords: 25 }}...
                        {% endif %}
                    </p>
                    
                    <!-- Terminal Prompt -->
                    <span class="text-amber-500 font-tech uppercase text-xs tracking-widest flex items-center gap-2">
                        <span class="text-amber-600 font-bold">&gt;_</span> Ler Capítulo
                    </span>
                </a>
            </div>
            {% endfor %}
        </div>
        
    </div>
</article>
