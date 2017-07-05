---
layout: post
title: "Numbers every C++ programmer should know"
date: 2017-07-07
---
<div class="css-full-post-content js-full-post-content">
<div dir="ltr" style="text-align: left;" trbidi="on">For everyone storing significant number of items in STL data structures.</div>


Data structure | Memory per element (bytes)
:---|:---
  vector(V) |  sizeof(V)                             
  unique_ptr(V) |  sizeof(V) + 8                         
  list(Value) |  sizeof(V) aligned to 8 + 16                     
  unordered_set(K)          |                         sizeof(K) aligned to 8 + 16           
 unordered_multiset(K)     |                          sizeof(K) aligned to 8 + 16           
 unordered_map(K, V)       |                          sizeof(pair(K, V)) aligned to 8 + 16  
  unordered_multimap(K, V)  |                          sizeof(pair(K, V)) aligned to 8 + 16  
  shared_ptr(V)             |                          sizeof(V) aligned to 8 + 32           
  set(V)                    |                          sizeof(V) aligned to 8 + 32           
  map(K,V)                  |                         sizeof(pair(K, V)) aligned to 8 + 32 

g++7 --std=c++14, x86_64
load factor 1.0 for unordered containers and vector (real world numbers will be a few bytes higher)
shared_ptr created with make_shared
</div>
