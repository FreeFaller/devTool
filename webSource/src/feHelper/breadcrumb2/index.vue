
<template>
	<Breadcrumb>
	    <BreadcrumbItem to="">Home222</BreadcrumbItem>
	    <BreadcrumbItem to="">Components</BreadcrumbItem>
	    <BreadcrumbItem>Breadcrumb</BreadcrumbItem>
	</Breadcrumb>
</template>
<script>
export default { 
	mounted(){
		console.log(666)
		console.warn('拿到cookie：'+ document.cookie)
	}
}
</script>

