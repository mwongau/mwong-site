<script>
const images = ["/mwong-site/acu1.jpg", "/mwong-site/uts5.jpg", "/mwong-site/hps1.jpg"]
const desc = [ "Australian Catholic University, Strathfield Campus, NSW, Australia",
	           "University of Technology Sydney, Building 5",
               "Homebush Public School, Homebush, NSW, Australia"]
const alts = ["ACU", "UTS", "Homebush Public School"]
let count = $state(0)

function next() {
    count = (count + 1) % images.length
}
</script> 

<h1 class="text-2xl font-bold my-3 text-purple-900" >Photos</h1>
<button onclick={next} class="m-2 p-1 font-bold bg-blue-200">Next photo</button>
<p class="my-2 font-bold">{desc[count]}</p>
<img src="{images[count]}" alt="{alts[count]}" />

