<script>
const images = ["/sv5site/acupy.jpg", "/sv5site/uts-bldg5.jpg", "/sv5site/hps.jpg"]
const desc = [ "Australian Catholic University, Strathfield Campus, NSW, Australia",
	          "University of Technology Sydney, Building 5",
              "Homebush Public School, Homebush, NSW, Australia"]
let count = $state(0)

function next() {
    count = (count + 1) % images.length
}
</script> 

<button onclick={next} class="m-2 p-1 font-bold bg-blue-200">Next photo</button>
<p class="my-2 font-bold">{desc[count]}</p>
<img src="{images[count]}" alt="image" />

