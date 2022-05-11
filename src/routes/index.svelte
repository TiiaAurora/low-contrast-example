<svelte:head>
	<title>Contrast Accessibility Demonstration | Text</title>
</svelte:head>

<p>
	This page is a demonstration on how you can implement a low contrast mode to help users with
	photosensitivity / photophobia. With a small JavaScript snippet, you can easily either create a
	toggle or buttons to switch between the two modes.
</p>
<p>
	For this demonstration the switch applies two filters to the entire page. The first one is a
	contrast filter set to 70%. The second one is a saturation filter set to 70%.
</p>
<p>For the CSS:</p>
<code class="inline-block p-6 bg-slate-600 rounded-lg">
	<pre>
<span class="text-yellow-400">body.lowcontrast &lcub;</span>
    filter: contrast(70%) saturate(70%);
<span class="text-yellow-400">&rcub;</span></pre>
</code>

<p>For the JavaScript:</p>

<code class="inline-block p-6 mt-4 bg-slate-600 rounded-lg">
	<pre>
<span class="text-blue-300">function</span> addLowContrast<span class="text-yellow-400"
			>() &lcub;</span
		>
    document.body.classList.add('lowcontrast');
<span class="text-yellow-400">&rcub;</span>

<span class="text-blue-300">function</span> removeLowContrast<span class="text-yellow-400"
			>() &lcub;</span
		>
    document.body.classList.remove('lowcontrast');
<span class="text-yellow-400">&rcub;</span></pre>
</code>

<p>Since this project uses Svelte, you can easily bind the functions to buttons with:</p>

<code class="inline-block p-6 mt-4 bg-slate-600 rounded-lg">
	<pre>
&lt;<span class="text-pink-400">button</span> on:click=<span class="text-yellow-400">&lcub;</span
		>addLowContrast<span class="text-yellow-400">&rcub;</span>&gt;Low Contrast&lt;/<span
			class="text-pink-400">button</span
		>&gt;

&lt;<span class="text-pink-400">button</span> on:click=<span class="text-yellow-400">&lcub;</span
		>removeLowContrast<span class="text-yellow-400">&rcub;</span>&gt;High Contrast&lt;/<span
			class="text-pink-400">button</span
		>&gt;</pre>
</code>

<p>
	The code is available on <a
		class="text-pink-400"
		href="https://github.com/TiiaAurora/low-contrast-example">GitHub</a
	>. A detailed blog post explaining the reasoning is available on
	<a
		class="text-pink-400"
		href="https://blog.tiia.rocks/web-apps-why-offering-a-low-contrast-mode-makes-you-more-accessible-not-less"
		>Hashnode</a
	>.
</p>
<h2>Example Text</h2>
<p>
	Lorem ipsum dolor, sit amet consectetur adipisicing elit. Aliquid minima quo distinctio, error hic
	iusto. Quisquam nobis, minus error vitae, nemo hic totam voluptatum ipsum cum quasi atque. Nisi,
	sint.
</p>
<p>
	Lorem ipsum dolor sit amet consectetur adipisicing elit. Incidunt laboriosam, sequi perferendis
	quis labore veniam omnis optio sit aspernatur, unde numquam id magni repudiandae, ullam vero
	ratione sunt? Minus impedit iusto voluptatum eligendi ea, autem incidunt! Sint quod, obcaecati eum
	eos id, ducimus sequi debitis optio earum expedita vitae delectus suscipit quisquam aliquam
	perferendis quia temporibus voluptates odio labore nobis laudantium iusto. Nostrum, impedit
	excepturi voluptatem dicta explicabo odit nihil animi nobis quam amet unde quia fugiat cum
	voluptas commodi odio magnam! Autem aliquid accusantium at enim adipisci corporis magni suscipit
	neque, inventore maxime?
</p>
