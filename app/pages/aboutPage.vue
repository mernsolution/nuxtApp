<template>
  <Nave />

  <div class="container mx-auto">
    <div class="grid grid-cols-2 mt-20">
      <div class="px-6">
       
        <div class="pt-4"> 
          <label>Your name </label>
          <input
          placeholder="input your name "
          class="placeholder:italic placeholder:text-slate-400 block bg-white w-full
           border border-slate-300 rounded-md py-2 pl-3 pr-3 shadow-sm focus:outline-none focus:border-sky-500
            focus:ring-sky-500 focus:ring-1 sm:text-sm"
          >
        
        </input>
        </div>
        
        <div class="pt-4">
          <label>Your Email</label>
          <input
          placeholder="input your Email "
          class="placeholder:italic placeholder:text-slate-400 block bg-white w-full
           border border-slate-300 rounded-md py-2 pl-3 pr-3 shadow-sm focus:outline-none focus:border-sky-500
            focus:ring-sky-500 focus:ring-1 sm:text-sm"
          >
        
        </input>
        </div>

        <div class="pt-4">
          <label>Your Phone Number</label>
          <input
          placeholder="input your Phone Number "
          class="placeholder:italic placeholder:text-slate-400 block bg-white w-full
           border border-slate-300 rounded-md py-2 pl-3 pr-3 shadow-sm focus:outline-none focus:border-sky-500
            focus:ring-sky-500 focus:ring-1 sm:text-sm"
          >
        
        </input>
        </div>
    
        <div class="pt-4">
          <label>Your Country</label>
          <input
          placeholder="input your country name "
          class="placeholder:italic placeholder:text-slate-400 block bg-white w-full
           border border-slate-300 rounded-md py-2 pl-3 pr-3 shadow-sm focus:outline-none focus:border-sky-500
            focus:ring-sky-500 focus:ring-1 sm:text-sm"
          >
        
        </input>
        </div>
    
        <div class="pt-4">
          <label>Your Zip Code</label>
          <input
          placeholder="input your Zip Code "
          class="placeholder:italic placeholder:text-slate-400 block bg-white w-full
           border border-slate-300 rounded-md py-2 pl-3 pr-3 shadow-sm focus:outline-none focus:border-sky-500
            focus:ring-sky-500 focus:ring-1 sm:text-sm"
          >
        
        </input>
        </div>
        <button
        class="bg-blue-600 mt-5 p-2 px-3 rounded-sm text-white"
        >Submit</button>
      </div>
      <div>
        <h2>hello there how are you</h2>
      </div>
    </div>
  </div>
</template>
