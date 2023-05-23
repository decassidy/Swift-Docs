<!DOCTYPE html>
<html>

<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Welcome file</title>
  <link rel="stylesheet" href="https://stackedit.io/style.css" />
</head>

<body class="stackedit">
  <div class="stackedit__left">
    <div class="stackedit__toc">
      
<ul>
<li><a href="#swift-5.8---coding-exercises---functions">Swift 5.8 - Coding Exercises - Functions</a>
<ul>
<li><a href="#defining-and-calling-functions">Defining and Calling Functions</a></li>
<li><a href="#functions-without-parameters">Functions Without Parameters</a></li>
<li><a href="#functions-with-multiple-parameters">Functions With Multiple Parameters</a></li>
<li><a href="#functions-without-return-values">Functions Without Return Values</a></li>
</ul>
</li>
</ul>

    </div>
  </div>
  <div class="stackedit__right">
    <div class="stackedit__html">
      <h1 id="swift-5.8---coding-exercises---functions">Swift 5.8 - Coding Exercises - Functions</h1>
<h2 id="defining-and-calling-functions">Defining and Calling Functions</h2>
<ol>
<li>
<p>Open a new playground in Xcode and name it “functions.playground”.</p>
</li>
<li>
<p>Write a function named “<code>greet</code>” and include parameter ("<code>person</code>") with a return type of <code>String</code>. The return will return the following string <code>"Hello, " + person + "!"</code></p>
</li>
</ol>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token comment">// Defining and calling functions</span>
<span class="token keyword">func</span> <span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token builtin">String</span><span class="token punctuation">)</span> <span class="token operator">-</span><span class="token operator">&gt;</span> <span class="token builtin">String</span> <span class="token punctuation">{</span>
	 <span class="token keyword">return</span> <span class="token string">"Hello, "</span> <span class="token operator">+</span> person <span class="token operator">+</span> <span class="token string">"!"</span>
 <span class="token punctuation">}</span>
</code></pre>
<ul>
<li>Call the function <code>greet</code> as in the example below:</li>
</ul>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token function">print</span><span class="token punctuation">(</span><span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token string">"Johnny"</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
 <span class="token comment">// prints - Hello, Johnny!</span>
</code></pre>
<ol start="3">
<li>Write a function named “<code>greetAgain</code>” and include parameter ("<code>person</code>") with a return type of <code>String</code>. The return will return the following string <code>"Hello, " + person + "1"</code>.</li>
</ol>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token keyword">func</span> <span class="token function">greetAgain</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token builtin">String</span><span class="token punctuation">)</span> <span class="token operator">-</span><span class="token operator">&gt;</span> <span class="token builtin">String</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token string">"Hello again, "</span> <span class="token operator">+</span> person <span class="token operator">+</span> <span class="token string">"!"</span>
 <span class="token punctuation">}</span>
</code></pre>
<ul>
<li>Call the function <code>greetAgain</code> as in the example below:</li>
</ul>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token function">print</span><span class="token punctuation">(</span><span class="token function">greetAgain</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token string">"Anna"</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
 <span class="token comment">// Prints "Hello again, Anna!"</span>
</code></pre>
<h2 id="functions-without-parameters">Functions Without Parameters</h2>
<ol>
<li>Write a function named “<code>sayHello</code>” without any parameters with a return type of <code>String</code>. The return will return the following string, <code>"Hello, Swift!"</code>.</li>
</ol>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token keyword">func</span> <span class="token function">sayHello</span><span class="token punctuation">(</span><span class="token punctuation">)</span> <span class="token operator">-</span><span class="token operator">&gt;</span> <span class="token builtin">String</span> <span class="token punctuation">{</span>
    <span class="token keyword">return</span> <span class="token string">"Hello, Swift!"</span>
 <span class="token punctuation">}</span>
</code></pre>
<ul>
<li>Call the function <code>sayHello</code> as in the example below:</li>
</ul>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token function">print</span><span class="token punctuation">(</span><span class="token function">sayhello</span><span class="token punctuation">(</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
 <span class="token comment">// Prints - Hello, Swift! </span>
</code></pre>
<h2 id="functions-with-multiple-parameters">Functions With Multiple Parameters</h2>
<ol>
<li>Write a function named “<code>greet</code>” and include the following parameters ("<code>person</code>" and “<code>alreadyGreeted</code>”) with a return type of <code>String</code>.</li>
</ol>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token keyword">func</span> <span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token builtin">String</span><span class="token punctuation">,</span> alreadyGreeted<span class="token punctuation">:</span> <span class="token builtin">Bool</span><span class="token punctuation">)</span> <span class="token operator">-</span><span class="token operator">&gt;</span> <span class="token builtin">String</span> <span class="token punctuation">{</span>
     <span class="token keyword">if</span> alreadyGreeted <span class="token punctuation">{</span>
         <span class="token keyword">return</span> <span class="token function">greetAgain</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> person<span class="token punctuation">)</span>
     <span class="token punctuation">}</span> <span class="token keyword">else</span> <span class="token punctuation">{</span>
         <span class="token keyword">return</span> <span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> person<span class="token punctuation">)</span>
     <span class="token punctuation">}</span>
 <span class="token punctuation">}</span>            
</code></pre>
<ul>
<li>Call the function <code>greet</code> as in the example below:</li>
</ul>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token function">print</span><span class="token punctuation">(</span><span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token string">"Johnny"</span><span class="token punctuation">,</span> alreadyGreeted<span class="token punctuation">:</span> <span class="token boolean">true</span><span class="token punctuation">)</span><span class="token punctuation">)</span>
 <span class="token comment">// Print "Hello again, Johnny!"</span>
</code></pre>
<h2 id="functions-without-return-values">Functions Without Return Values</h2>
<ol>
<li>Write a function named “<code>greet</code>” and include the following parameter ("<code>person</code>") with no return type.</li>
</ol>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token keyword">func</span> <span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token builtin">String</span><span class="token punctuation">)</span> <span class="token punctuation">{</span>
     <span class="token function">print</span><span class="token punctuation">(</span><span class="token string">"Hello, <span class="token interpolation"><span class="token delimiter variable">\(</span>person<span class="token delimiter variable">)</span></span>!"</span><span class="token punctuation">)</span>
 <span class="token punctuation">}</span>
</code></pre>
<ul>
<li>Call the function <code>greet</code> as in the example below:</li>
</ul>
<pre class=" language-swift"><code class="prism  language-swift"><span class="token function">greet</span><span class="token punctuation">(</span>person<span class="token punctuation">:</span> <span class="token string">"Dave"</span><span class="token punctuation">)</span>
 <span class="token comment">// Prints "Hello, Dave!"</span>
</code></pre>

    </div>
  </div>
</body>

</html>
