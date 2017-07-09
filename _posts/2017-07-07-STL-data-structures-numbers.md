---
layout: post
title: "Numbers every C++ programmer should know"
date: 2017-07-07
---
<div class="css-full-post-content js-full-post-content">
<div dir="ltr" style="text-align: left;" trbidi="on">For everyone storing significant number of items in STL data structures.</div>

<table>
<thead>
<tr><th>Data structure</th><th>Memory per element (bytes)</th></tr>
</thead>
<tbody align="center">
<tr><td>vector(V)</td><td>sizeof(V)</td></tr>                             
<tr><td>unique_ptr(V)</td><td>sizeof(V) + 8</td></tr>
<tr><td>list(Value)</td><td>sizeof(V) aligned to 8 + 16</td></tr>                    
<tr><td>unordered_set(K)</td><td>sizeof(K) aligned to 8 + 16</td></tr>          
<tr><td>unordered_multiset(K)</td><td>sizeof(K) aligned to 8 + 16</td></tr>         
<tr><td>unordered_map(K, V)</td><td>sizeof(pair(K, V)) aligned to 8 + 16</td></tr>
<tr><td>unordered_multimap(K, V)</td><td>sizeof(pair(K, V)) aligned to 8 + 16</td></tr>
<tr><td>shared_ptr(V)</td><td>sizeof(V) aligned to 8 + 32</td></tr>
<tr><td>set(V)</td><td>sizeof(V) aligned to 8 + 32</td></tr>          
<tr><td>map(K,V)</td><td>sizeof(pair(K, V)) aligned to 8 + 32</td></tr>
</tbody>
</table>

</div>
