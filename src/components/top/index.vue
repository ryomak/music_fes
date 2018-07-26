<template>
	<div>
		<main-component id="sec01"/>
		<about id="sec02" />
		<schedule id="sec03"/>
		<gallery id="sec04"/>
		<contact id="sec05"/>
		<place id="sec06"/>
	</div>
</template>
<script>
import MainComponent  from "@/components/top/main"
import About from "@/components/top/about"
import Contact from "@/components/top/contact"
import Place from "@/components/top/place"
import Gallery from "@/components/top/gallery"
import Schedule from "@/components/top/schedule"
export default{
	name:"Top",
	components:{
		MainComponent,
		About,
		Contact,
		Place,
		Gallery,
		Schedule,
	}
}
	
</script>