
<template>
	<Table height="200"  :columns="FEHPVBcolumns1" :data="FEHPVBdata1"></Table>
</template>
<script>
export default { 
	
	data(){
		return {
			FEHPVBcolumns1: [
                    {
                        title: 'Name',
                        key: 'name'
                    },
                    {
                        title: 'Age',
                        key: 'age'
                    }
                ],
                FEHPVBdata1: [
                    {
                        name: 'John Brown',
                        age: 18
                    }
                ]
		}
	}
}
</script>
