<!-- 
	This is the default layout, used in sign-in and sign-up pages.
 -->

<template>
	<div>

		<!-- Default Layout -->
		<a-layout class="layout-default" id="layout-default" :class="['layout-default']">
			<!-- Layout Header ( Navbar ) -->
			<DefaultHeader></DefaultHeader>
			<!-- / Layout Header ( Navbar ) -->


			<!-- Page Content -->
			<a-layout-content>
        <router-view />
			</a-layout-content>
			<!-- / Page Content -->

			<!-- Layout Footer -->
			<DefaultFooter></DefaultFooter>
			<!-- / Layout Footer -->

		</a-layout>
		<!-- / Default Layout -->

	</div>
</template>

<script>

	import DefaultHeader from '../components/Headers/DefaultHeader' ;
	import DefaultFooter from '../components/Footers/DefaultFooter' ;
	export default ({
		components: {
			DefaultHeader,
			DefaultFooter,
		},
		data() {
			return {
			}
		},
	})

</script>
