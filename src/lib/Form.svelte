<!-- src/lib/Form.svelte -->
<script>
  import LoadingIndicator from './Loading.svelte';

  // List of favorite venues (restaurants, bars, etc.)
  let venues = [
    // Example: { name: 'Venue Name', type: 'Restaurant', walkingDistance: true }
  ];
  let selectedVenues = [];
  let walkingDistance = false;

  function selectVenue(venue) {
    selectedVenues.push(venue);
  }
</script>

<div class="pt-6 md:pt-10 text-slate-200">
  <div>
    
    <div class="mt-8">
		<input
		class="relative float-left -ml-[1.5rem] mr-[6px] mt-[0.15rem] h-[1.125rem] w-[1.125rem] appearance-none rounded-[0.25rem] border-[0.125rem] border-solid border-neutral-300 outline-none before:pointer-events-none before:absolute before:h-[0.875rem] before:w-[0.875rem] before:scale-0 before:rounded-full before:bg-transparent before:opacity-0 before:shadow-[0px_0px_0px_13px_transparent] before:content-[''] checked:border-primary checked:bg-primary checked:before:opacity-[0.16] checked:after:absolute checked:after:-mt-px checked:after:ml-[0.25rem] checked:after:block checked:after:h-[0.8125rem] checked:after:w-[0.375rem] checked:after:rotate-45 checked:after:border-[0.125rem] checked:after:border-l-0 checked:after:border-t-0 checked:after:border-solid checked:after:border-white checked:after:bg-transparent checked:after:content-[''] hover:cursor-pointer hover:before:opacity-[0.04] hover:before:shadow-[0px_0px_0px_13px_rgba(0,0,0,0.6)] focus:shadow-none focus:transition-[border-color_0.2s] focus:before:scale-100 focus:before:opacity-[0.12] focus:before:shadow-[0px_0px_0px_13px_rgba(0,0,0,0.6)] focus:before:transition-[box-shadow_0.2s,transform_0.2s] focus:after:absolute focus:after:z-[1] focus:after:block focus:after:h-[0.875rem] focus:after:w-[0.875rem] focus:after:rounded-[0.125rem] focus:after:content-[''] checked:focus:before:scale-100 checked:focus:before:shadow-[0px_0px_0px_13px_#3b71ca] checked:focus:before:transition-[box-shadow_0.2s,transform_0.2s] checked:focus:after:-mt-px checked:focus:after:ml-[0.25rem] checked:focus:after:h-[0.8125rem] checked:focus:after:w-[0.375rem] checked:focus:after:rotate-45 checked:focus:after:rounded-none checked:focus:after:border-[0.125rem] checked:focus:after:border-l-0 checked:focus:after:border-t-0 checked:focus:after:border-solid checked:focus:after:border-white checked:focus:after:bg-transparent dark:border-neutral-600 dark:checked:border-primary dark:checked:bg-primary dark:focus:before:shadow-[0px_0px_0px_13px_rgba(255,255,255,0.4)] dark:checked:focus:before:shadow-[0px_0px_0px_13px_#3b71ca]"
		type="checkbox"
		value=""
		id="checkboxDefault" />
	  <label
		class="inline-block pl-[0.15rem] hover:cursor-pointer"
		for="checkboxDefault">Walking Distance
	  </label>
      <button
        on:click
        class="bg-pink-600 hover:bg-gradient-to-r from-pink-700 via-pink-600 to-pink-700 mt-4 w-full h-10 text-white font-bold p-3 rounded-full flex items-center justify-center"
      >
        <p>Generate Date Ideas</p>
      </button>
    </div>
  </div>
</div>
