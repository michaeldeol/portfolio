---
layout: page
title: Blog
permalink: /blog/
---

<div class="grid gap-8 md:gap-12">
  {%- if site.posts.size > 0 -%}
    {%- for post in site.posts -%}
    <article class="bg-slate-800 border border-slate-700 rounded-lg overflow-hidden hover:border-slate-600 transition-colors">
      <div class="p-8">
        <div class="flex flex-wrap gap-2 mb-4">
          {%- for tag in post.tags -%}
          <span class="px-3 py-1 text-xs font-medium bg-indigo-600/20 text-indigo-300 rounded-full">
            {{ tag }}
          </span>
          {%- endfor -%}
        </div>
        
        <h2 class="text-2xl font-bold text-white mb-4">
          <a href="{{ post.url | relative_url }}" class="hover:text-indigo-400 transition-colors">
            {{ post.title | escape }}
          </a>
        </h2>
        
        <div class="flex items-center text-slate-400 text-sm mb-4">
          <time datetime="{{ post.date | date_to_xmlschema }}">
            {{ post.date | date: "%B %d, %Y" }}
          </time>
          {%- if post.author -%}
          <span class="mx-2">•</span>
          <span>{{ post.author }}</span>
          {%- endif -%}
        </div>
        
        {%- if post.excerpt -%}
        <div class="text-slate-300 mb-6 prose prose-invert max-w-none">
          {{ post.excerpt }}
        </div>
        {%- endif -%}
        
        <a href="{{ post.url | relative_url }}" class="inline-flex items-center text-indigo-400 hover:text-indigo-300 font-medium transition-colors">
          Read Full Post
          <svg class="ml-2 w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 8l4 4m0 0l-4 4m4-4H3"></path>
          </svg>
        </a>
      </div>
    </article>
    {%- endfor -%}
  {%- else -%}
    <div class="text-center py-20">
      <div class="max-w-md mx-auto">
        <svg class="mx-auto h-12 w-12 text-slate-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
          <path stroke-linecap="round" stroke-linejoin="round" stroke-width="1" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
        </svg>
        <h3 class="mt-4 text-lg font-medium text-white">No blog posts yet</h3>
        <p class="mt-2 text-slate-400">Check back soon for new content!</p>
      </div>
    </div>
  {%- endif -%}
</div>