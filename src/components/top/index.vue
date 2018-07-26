<template>
	<div>
		<main-component id="sec01"/>
		<about id="sec02" />
		<gallery id="sec03"/>
		<contact id="sec04"/>
		<place id="sec05"/>
	</div>
</template>
<script>
import MainComponent  from "@/components/top/main"
import About from "@/components/top/about"
import Contact from "@/components/top/contact"
import Place from "@/components/top/place"
import Gallery from "@/components/top/gallery"
export default{
	name:"Top",
	components:{
		MainComponent,
		About,
		Contact,
		Place,
		Gallery,
	}
}
	
</script>