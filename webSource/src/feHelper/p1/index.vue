
<template>
	<div>
		<Breadcrumb>
		    <BreadcrumbItem to="">Home</BreadcrumbItem>
		    <BreadcrumbItem>Breadcrumb</BreadcrumbItem>
		</Breadcrumb>
		<FEHPVBSearchBar 
	        :searchElems="FEHPVBsearchElems" 
	        :serachValue="FEHPVBserachValue"
	        @search="FEHPVBsearch"
	        @reset="FEHPVBreset"
	    />
	    <Table :columns="FEHPVBcolumns1" :data="FEHPVBdata1"></Table>
	    <Page :total="100" show-elevator show-sizer show-total />
	</div>
</template>
<script>
import FEHPVBSearchBar from '@feHelper/searchBar1-base/index.vue'
export default { 
	data(){
		return{
			FEHPVBsearchElems: [
                {
                    title: '业务选项',
                    key: 'business',
                    type: 'radio',
                    items: [
                        {label: '全部', value: 1}
                    ]
                },
                {
                    title: '所在区域',
                    key: 'cityId',
                    type: 'select',
                    items: [
                        {label: '全部', value: 1}
                    ]
                },
                {
                    key: 'idcName',
                    type: 'input',
                    title: '机房名称',
                    placeholder: '输入关键字进行搜索'
                }
            ],
            FEHPVBserachValue:{
                business: 1,
            },
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
	},
    methods:{
        FEHPVBsearch(v){
            
        },

        FEHPVBreset(v){
            
        },
        
    },
    components:{
        FEHPVBSearchBar
    }
}
</script>

