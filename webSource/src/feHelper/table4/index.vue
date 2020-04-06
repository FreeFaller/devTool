
<template>
    <Table :columns="FEHPVBcolumns" :data="FEHPVBdata">
    <template slot-scope="{ row, index }" slot="action">
        <Button type="primary"  @click="">click</Button>
    </template>
</Table>
</template>
<script>
export default { 
	
	data(){
		return {
			FEHPVBcolumns: [
                    {
                        title: 'Name',
                        key: 'name'
                    },
                    {
                        title: 'Age',
                        key: 'age'
                    },
                    {
                        title: 'Action',
                        slot: 'action',
                        width: 150,
                        align: 'center'
                    }
                ],
                FEHPVBdata: [
                    {
                        name: 'John',
                        age: 18
                    },
                ]
		}
	}
}
</script>
