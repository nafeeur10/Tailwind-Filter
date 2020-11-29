<template>
  <div class="custom-filter">
    <nav id="header" class="fixed w-full">
    <!--Nav-->
    <div class="relative w-full z-10 fixed top-0 bg-gray-200 border-b border-grey-light">
      <div class="w-full container mx-auto flex flex-wrap items-center justify-between mt-0 py-4">
        <div class="flex items-center">
          <a class="text-teal-700 text-base no-underline hover:no-underline font-extrabold text-xl" href="#"> Search and Filter</a>
        </div>

        <div class="pr-4">
          <button id="nav-toggle" class="block lg:hidden flex items-center px-3 py-2 border rounded text-grey border-grey-dark hover:text-black hover:border-purple appearance-none focus:outline-none">
            <svg class="fill-current h-3 w-3" viewBox="0 0 20 20" xmlns="http://www.w3.org/2000/svg"><title>Menu</title><path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z"></path></svg>
          </button>
        </div>

      </div>
    </div>


    <div class="absolute mt-3 px-2 w-screen ml-8 pr-16">
      <div class="rounded-lg shadow-lg ring-1 ring-black ring-opacity-5">
        <div class="relative grid gap-6 bg-white px-5 py-6 sm:gap-8 sm:p-8">
          <div class="-m-3 p-3 flex items-start rounded-lg">
            <div class="ml-4 w-full flex">
              <div class="pt-2 relative text-gray-600 mr-4">
                <button type="submit" class="absolute left-4 top-0 mt-5 mr-4">
                  <svg class="text-gray-600 h-4 w-4 fill-current" xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px"
                    viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 56.966 56.966;" xml:space="preserve"
                    width="512px" height="512px">
                    <path
                      d="M55.146,51.887L41.588,37.786c3.486-4.144,5.396-9.358,5.396-14.786c0-12.682-10.318-23-23-23s-23,10.318-23,23  s10.318,23,23,23c4.761,0,9.298-1.436,13.177-4.162l13.661,14.208c0.571,0.593,1.339,0.92,2.162,0.92  c0.779,0,1.518-0.297,2.079-0.837C56.255,54.982,56.293,53.08,55.146,51.887z M23.984,6c9.374,0,17,7.626,17,17s-7.626,17-17,17  s-17-7.626-17-17S14.61,6,23.984,6z" />
                  </svg>
                </button>
                <input class="border-2 border-gray-300 bg-white h-10 px-5 pl-10 rounded-full text-sm focus:outline-none"
                  type="search" 
                  name="search" 
                  placeholder="Search Name, ID..."
                >
              </div>

              <div class="pt-2 relative text-gray-600">
                <button type="submit" class="absolute left-4 top-0 mt-5 mr-4">
                  <svg class="text-gray-600 h-4 w-4 fill-current" xmlns="http://www.w3.org/2000/svg"
                    xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" id="Capa_1" x="0px" y="0px"
                    viewBox="0 0 56.966 56.966" style="enable-background:new 0 0 56.966 56.966;" xml:space="preserve"
                    width="512px" height="512px">
                    <path
                      d="M55.146,51.887L41.588,37.786c3.486-4.144,5.396-9.358,5.396-14.786c0-12.682-10.318-23-23-23s-23,10.318-23,23  s10.318,23,23,23c4.761,0,9.298-1.436,13.177-4.162l13.661,14.208c0.571,0.593,1.339,0.92,2.162,0.92  c0.779,0,1.518-0.297,2.079-0.837C56.255,54.982,56.293,53.08,55.146,51.887z M23.984,6c9.374,0,17,7.626,17,17s-7.626,17-17,17  s-17-7.626-17-17S14.61,6,23.984,6z" />
                  </svg>
                </button>
                <input class="border-2 border-gray-300 bg-white h-10 px-5 pl-10 rounded-full text-sm focus:outline-none"
                  type="search" 
                  name="search" 
                  placeholder="Search Name, ID..."
                >
              </div>
            </div>
          </div>

          <div class="-m-3 p-3 flex items-start rounded-lg">
            <div class="ml-4 w-full flex">
              <div class="pt-2 relative text-gray-600 mr-4">
                <button type="submit" class="absolute left-4 top-0 mt-5 mr-4">
                  <svg style="width: 20px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M3 3a1 1 0 011-1h12a1 1 0 011 1v3a1 1 0 01-.293.707L12 11.414V15a1 1 0 01-.293.707l-2 2A1 1 0 018 17v-5.586L3.293 6.707A1 1 0 013 6V3z" clip-rule="evenodd" />
                  </svg>
                </button>
                <button type="button" class="pl-12 inline-flex justify-center w-full rounded-full border border-gray-300 shadow-sm px-4 py-2 bg-gray-300 text-sm font-medium text-gray-700 hover:bg-gray-50" id="options-menu" aria-haspopup="true" aria-expanded="true">
                  Filter
                  <svg class="-mr-1 ml-2 h-5 w-5" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                    <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                </button>
              </div>

              <div class="pt-2 relative text-gray-600">
                <button type="submit" class="absolute left-4 top-0 mt-5 mr-4">
                  <svg style="width: 20px" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor">
                    <path fill-rule="evenodd" d="M3 3a1 1 0 011-1h12a1 1 0 011 1v3a1 1 0 01-.293.707L12 11.414V15a1 1 0 01-.293.707l-2 2A1 1 0 018 17v-5.586L3.293 6.707A1 1 0 013 6V3z" clip-rule="evenodd" />
                  </svg>
                </button>
                <button 
                  type="button" 
                  class="active:outline-none active:border-opacity-0 pl-12 inline-flex justify-center w-full rounded-full border border-gray-300 shadow-sm px-4 py-2 bg-gray-300 text-sm font-medium text-gray-700 hover:bg-gray-50" 
                  id="filter-menu" 
                  aria-haspopup="true" 
                  aria-expanded="true"
                  @click="searchOptions"
                >
                  Filter
                  <svg class="-mr-1 ml-2 h-5 w-5" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20" fill="currentColor" aria-hidden="true">
                    <path fill-rule="evenodd" d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z" clip-rule="evenodd" />
                  </svg>
                </button>
                <div :class="{ hidden : !activeSearchBar }" class="origin-top-right absolute mt-2 w-screen max-w-4xl sm:px-0 lg:ml-0 lg:-translate-x-3/4 rounded-md shadow-lg bg-white ring-1 ring-black ring-opacity-5">
                  <div class="p-4" role="menu" aria-orientation="vertical" aria-labelledby="filter-menu">
                    <div class="flex justify-between">
                      <div>
                        <span><b>Fleets</b></span>
                        <div class="block">
                          <label class="flex items-center my-2" v-for="fleet in fleets" :key="fleet.id">
                            <input type="checkbox" class="form-checkbox h-4 w-4 text-gray-900" :checked="fleet.checked">
                            <span class="ml-2">{{ fleet.name }}</span>
                          </label>
                        </div>
                      </div>

                      <div>
                        <span><b>Currency</b></span>
                        <div class="block">
                          <label class="flex items-center my-2" v-for="currency in currencies" :key="currency.id">
                            <input type="checkbox" class="form-checkbox h-4 w-4 text-gray-900" :checked="currency.checked">
                            <span class="ml-2">{{ currency.name }}</span>
                          </label>
                        </div>
                      </div>

                      <div>
                        <span><b>Rating</b></span>
                        <div class="block">
                          <label class="flex items-center my-2" v-for="rating in ratings" :key="rating.id">
                            <input type="radio" v-model="ratingModel" :value="rating.value" name="rating" class="form-radio h-4 w-4 text-gray-900">
                            <span class="ml-2">{{ rating.name }}</span>
                          </label>
                        </div>

                        <span><b>Gender</b></span>
                        <div class="block">
                          <label class="flex items-center my-2" v-for="sex in gender" :key="sex.id">
                            <input type="radio" name="gender" :value="sex.value" v-model="genderModel" class="form-radio h-4 w-4 text-gray-900">
                            <span class="ml-2">{{ sex.name }}</span>
                          </label>
                        </div>
                      </div>

                      <div>
                        <span><b>Range</b></span>
                        <div class="block">
                          <label class="flex items-center my-2" v-for="range in allrange" :key="range.id">
                            <input type="checkbox" class="form-checkbox h-4 w-4 text-gray-900" :checked="range.checked">
                            <span class="ml-2">{{ range.name }}</span>
                          </label>
                        </div>
                      </div>

                      <div>
                        <span><b>Custom Range</b></span>
                        <div class="block">
                          <div class="range-slider">
                            <input @change="slider" v-model.number="minPrice" min="0" max="120000" step="500" type="range" />
                            <input @change="slider" v-model.number="maxPrice" min="0" max="120000" step="500" type="range" />
                          </div>

                          <div class="flex">
                            <div class="mt-4 border-2 p-4 mr-4">
                              <span class="block">Min Amount</span>
                              <span>${{ minPrice }}</span>
                            </div>

                            <div class="mt-4 border-2 p-4">
                              <span class="block">Max Amount</span>
                              <span>${{ maxPrice }}</span>
                            </div>
                          </div>
                          
                        </div>
                      </div>
                    </div>
                    <div class="flex float-right">
                      <button class="float-right border border-green-500 bg-green-500 text-white rounded-md px-4 py-2 m-2 transition duration-500 ease select-none hover:bg-green-600 focus:outline-none focus:shadow-outline">APPLY FILTER</button>
                      <button class="float-right border border-gray-200 bg-gray-200 text-gray-700 rounded-md px-4 py-2 m-2 transition duration-500 ease select-none hover:bg-gray-300 focus:outline-none focus:shadow-outline">CLEAR</button>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>

  </nav>

  </div>
</template>

<script>
export default {
  name: 'CustomFilter',
  data() {
    return {
      activeSearchBar: false,
      genderModel: 'male',
      ratingModel: 'good',
      fleets: [
        { id: 1, name: 'All Fleets', checked: false},
        { id: 2, name: 'Gulshan 1', checked: true},
        { id: 3, name: 'Gulshan 2', checked: true},
        { id: 4, name: 'Baridhara', checked: false},
        { id: 5, name: 'Badda', checked: true},
        { id: 6, name: 'Rampura', checked: false},
        { id: 7, name: 'Mouchak', checked: true},
        { id: 8, name: 'Merul', checked: false},
        { id: 9, name: 'Link Road', checked: true}
      ],
      currencies: [
        { id: 1, name: 'All', checked: false},
        { id: 2, name: 'USD', checked: true},
        { id: 3, name: 'EURO', checked: true},
        { id: 4, name: 'USD', checked: false},
        { id: 5, name: 'EURO', checked: true}
      ],
      ratings: [
        { id: 1, name: 'All', value: 'all'},
        { id: 2, name: 'Good', value: 'good'},
        { id: 3, name: 'Bad', value: 'bad'}
      ],
      gender: [
        { id: 1, name: 'All', value: 'all'},
        { id: 2, name: 'Male', value: 'male'},
        { id: 3, name: 'Female', value: 'female'}
      ],
      allrange: [
        { id: 1, name: 'All Range', checked: false},
        { id: 2, name: '10 - 20', checked: true},
        { id: 3, name: '20 - 30', checked: true},
        { id: 4, name: '30 - 40', checked: false}
      ],
      minPrice: "500",
      maxPrice: "50000",
      minValue: "25000"
    }
  },
  methods: {
    searchOptions() {
      this.activeSearchBar = !this.activeSearchBar
    },
    hideSearchOptions() {
      this.activeSearchBar = false
    },
    slider() {
      if (this.minPrice > this.maxPrice) {
        var tmp = this.maxPrice;
        this.maxPrice = this.minPrice;
        this.minPrice = tmp;
      }
    }
  }
}
</script>

<style>
button:focus {
    outline: 1px dotted;
    outline: 0px auto -webkit-focus-ring-color!important;
}

@media screen and (-webkit-min-device-pixel-ratio: 0) {
    input[type="range"]::-webkit-slider-thumb {
        width: 15px;
        -webkit-appearance: none;
        appearance: none;
        height: 15px;
        cursor: ew-resize;
        background: #FFF;
        box-shadow: -405px 0 0 400px #605E5C;
        border-radius: 50%;
        
    }
}

.range-slider {
  width: 300px;
  margin: auto;
  text-align: center;
  position: relative;
  height: 2em;
}

.range-slider svg,
.range-slider input[type=range] {
  position: absolute;
  left: 0;
  bottom: 0;
}

input[type=number] {
  border: 1px solid #ddd;
  text-align: center;
  font-size: 1.6em;
  -moz-appearance: textfield;
}

input[type=number]::-webkit-outer-spin-button,
input[type=number]::-webkit-inner-spin-button {
  -webkit-appearance: none;
}

input[type=number]:invalid,
input[type=number]:out-of-range {
  border: 2px solid #ff6347;
}

input[type=range] {
  -webkit-appearance: none;
  width: 100%;
}

input[type=range]:focus {
  outline: none;
}

input[type=range]:focus::-webkit-slider-runnable-track {
  background: #2497e3;
}

input[type=range]:focus::-ms-fill-lower {
  background: #2497e3;
}

input[type=range]:focus::-ms-fill-upper {
  background: #2497e3;
}

input[type=range]::-webkit-slider-runnable-track {
  width: 100%;
  height: 5px;
  cursor: pointer;
  animate: 0.2s;
  background: #2497e3;
  border-radius: 1px;
  box-shadow: none;
  border: 0;
}

input[type=range]::-webkit-slider-thumb {
  z-index: 2;
  position: relative;
  box-shadow: 0px 0px 0px #000;
  border: 1px solid #2497e3;
  height: 18px;
  width: 18px;
  border-radius: 25px;
  background: #a1d0ff;
  cursor: pointer;
  -webkit-appearance: none;
  margin-top: -7px;
}

</style>
