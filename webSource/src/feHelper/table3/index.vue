
<template>
	<Table width="250" border :columns="FEHPVBcolumns" :data="FEHPVBdata"></Table>
</template>
<script>
export default { 
	
	data(){
		return {
			FEHPVBcolumns: [
                    {
                        title: 'Name',
                        key: 'name',
                        width: 100,
                        fixed: 'left'
                    },
                    {
                        title: 'Age',
                        key: 'age',
                        width: 100
                    },
                    {
                        title: 'Province',
                        key: 'province',
                        width: 100,
                        fixed: 'right'
                    }
                ],
                FEHPVBdata: [
                    {
                        name: 'John Brown',
                        age: 18,
                        province: 'America'
                    },
                ]
		}
	}
}
</script>
