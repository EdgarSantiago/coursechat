<script lang="ts">
	import { spring } from 'svelte/motion';

	let count = 0;

	const displayed_count = spring();
	$: displayed_count.set(count);
	$: offset = modulo($displayed_count, 1);

	function modulo(n: number, m: number) {
		// handle negative numbers
		return ((n % m) + m) % m;
	}
</script>

<div class="testimonial border-2 bg-white border-green-100 rounded-md shadow-md p-8">
	<div class="mx-auto text-center md:max-w-xl lg:max-w-3xl">
		<h3
		  class="mb-6 text-3xl font-bold text-neutral-800 dark:text-neutral-200">
		  What Our Readers Have to Say
		</h3>
		<p class="mb-6 pb-2 md:mb-12 md:pb-0">
		  Lorem ipsum dolor sit amet, consectetur adipisicing elit. Fugit, error
		  amet numquam iure provident voluptate esse quasi, veritatis totam
		  voluptas nostrum quisquam eum porro a pariatur veniam.
		</p>
	  </div>
	  
	  <!-- Container for the Testimonials -->
	  <div class="grid gap-6 text-center md:grid-cols-3 lg:gap-12">
		<!-- Second Testimonial -->
		<div class="mb-12 md:mb-0">
		  <div class="mb-6 flex justify-center">
			<img
			  src="/john.jpg"
			  class="w-32 rounded-full shadow-lg dark:shadow-black/30" alt="1"/>
		  </div>
		  <h5 class="mb-4 text-xl font-semibold">John D, Investor</h5>
		 
		  <p class="mb-4 text-neutral-600">
			<svg
			  xmlns="http://www.w3.org/2000/svg"
			  fill="currentColor"
			  class="inline-block h-7 w-7 pr-2"
			  viewBox="0 0 24 24">
			  <path
				d="M13 14.725c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275zm-13 0c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275z" />
			</svg>
			Reading this eBook was a game-changer for me. As an investor, I'm always looking for new ways to identify opportunities and stay ahead of the curve. The insights and strategies presented in 'The Future of Wealth: How to make money with ChatGPT' have helped me do just that. Highly recommend!
		  </p>
		  <ul class="mb-0 flex items-center justify-center">
			<li>
			  <svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 24 24"
				fill="currentColor"
				class="h-5 w-5 text-yellow-500">
				<path
				  fill-rule="evenodd"
				  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
				  clip-rule="evenodd" />
			  </svg>
			</li>
			<li>
			  <svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 24 24"
				fill="currentColor"
				class="h-5 w-5 text-yellow-500">
				<path
				  fill-rule="evenodd"
				  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
				  clip-rule="evenodd" />
			  </svg>
			</li>
			<li>
			  <svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 24 24"
				fill="currentColor"
				class="h-5 w-5 text-yellow-500">
				<path
				  fill-rule="evenodd"
				  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
				  clip-rule="evenodd" />
			  </svg>
			</li>
			<li>
			  <svg
				xmlns="http://www.w3.org/2000/svg"
				viewBox="0 0 24 24"
				fill="currentColor"
				class="h-5 w-5 text-yellow-500">
				<path
				  fill-rule="evenodd"
				  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
				  clip-rule="evenodd" />
			  </svg>
			</li>
			<li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
		
		  </ul>
		</div>
	  
		<!-- Third Testimonial -->
		<div class="mb-0">
		  <div class="mb-12 md:mb-0">
			<div class="mb-6 flex justify-center">
			  <img
				src="/sarah.jpg"
				class="w-32 rounded-full shadow-lg dark:shadow-black/30"  alt="2">
				
			</div>
			<h5 class="mb-4 text-xl font-semibold">Sarah M, Entrepreneur</h5>
			
			<p class="mb-4 text-neutral-600 dark:text-neutral-300">
			  <svg
				xmlns="http://www.w3.org/2000/svg"
				fill="currentColor"
				class="inline-block h-7 w-7 pr-2"
				viewBox="0 0 24 24">
				<path
				  d="M13 14.725c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275zm-13 0c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275z" />
			  </svg>
			  I never knew how powerful AI could be until I read this eBook. The author does an excellent job of explaining the role of ChatGPT in wealth creation and how to leverage its capabilities. I'm excited to start exploring the new opportunities that AI can offer, and this eBook was the perfect starting point.
			</p>
			<ul class="mb-0 flex items-center justify-center">
			  <li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
			  <li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
			  <li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
			  <li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
			  <li>
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  viewBox="0 0 24 24"
				  fill="currentColor"
				  class="h-5 w-5 text-yellow-500">
				  <path
					fill-rule="evenodd"
					d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					clip-rule="evenodd" />
				</svg>
			  </li>
			</ul>
		  </div>
		</div>
		<!--  -->
		<div class="mb-0">
			<div class="mb-12 md:mb-0">
			  <div class="mb-6 flex justify-center">
				<img
				  src="david.jpg"
				  class="w-32 rounded-full shadow-lg dark:shadow-black/30" 
				  alt="3"/>
			  </div>
			  <h5 class="mb-4 text-xl font-semibold">David S, Business Owner</h5>
			
			  <p class="mb-4 text-neutral-600 dark:text-neutral-300">
				<svg
				  xmlns="http://www.w3.org/2000/svg"
				  fill="currentColor"
				  class="inline-block h-7 w-7 pr-2"
				  viewBox="0 0 24 24">
				  <path
					d="M13 14.725c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275zm-13 0c0-5.141 3.892-10.519 10-11.725l.984 2.126c-2.215.835-4.163 3.742-4.38 5.746 2.491.392 4.396 2.547 4.396 5.149 0 3.182-2.584 4.979-5.199 4.979-3.015 0-5.801-2.305-5.801-6.275z" />
				</svg>
				If you're looking for a new way to create wealth, this eBook is a must-read. The author provides a wealth of knowledge and strategies for using ChatGPT to generate new business ideas, investment opportunities, and more. I was blown away by the potential of AI and how it can be used to transform the world of wealth creation.
			  </p>
			  <ul class="mb-0 flex items-center justify-center">
				<li>
				  <svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5 text-yellow-500">
					<path
					  fill-rule="evenodd"
					  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					  clip-rule="evenodd" />
				  </svg>
				</li>
				<li>
				  <svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5 text-yellow-500">
					<path
					  fill-rule="evenodd"
					  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					  clip-rule="evenodd" />
				  </svg>
				</li>
				<li>
				  <svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5 text-yellow-500">
					<path
					  fill-rule="evenodd"
					  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					  clip-rule="evenodd" />
				  </svg>
				</li>
				<li>
				  <svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5 text-yellow-500">
					<path
					  fill-rule="evenodd"
					  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					  clip-rule="evenodd" />
				  </svg>
				</li>
				<li>
				  <svg
					xmlns="http://www.w3.org/2000/svg"
					viewBox="0 0 24 24"
					fill="currentColor"
					class="h-5 w-5 text-yellow-500">
					<path
					  fill-rule="evenodd"
					  d="M10.788 3.21c.448-1.077 1.976-1.077 2.424 0l2.082 5.007 5.404.433c1.164.093 1.636 1.545.749 2.305l-4.117 3.527 1.257 5.273c.271 1.136-.964 2.033-1.96 1.425L12 18.354 7.373 21.18c-.996.608-2.231-.29-1.96-1.425l1.257-5.273-4.117-3.527c-.887-.76-.415-2.212.749-2.305l5.404-.433 2.082-5.006z"
					  clip-rule="evenodd" />
				  </svg>
				</li>
			  </ul>
			</div>
		  </div>
	  </div>
</div>

<style>

</style>
