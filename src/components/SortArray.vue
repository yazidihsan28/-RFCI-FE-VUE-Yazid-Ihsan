<template>
    <div class="container py-4">
        <ol>
            <!-- <li v-repeat="items">
                [{{items}}]
            </li> -->
           <li>
               [7,9] -> {{item1}}
           </li>  
           <li>
               [5,9] -> {{item2}}
           </li>  
            <li>
               [5,7] -> {{item3}}
           </li>  
            <li>
               [8,9] -> {{item4}}
           </li>  
            <li>
               [3,9] -> {{item5}}
           </li>  
            <li>
               [3,9] -> {{item6}}
           </li>  
            <li>
               [3,8] -> {{item7}}
           </li>  
            <li>
               [3,7] -> {{item8}}
           </li>  
            <li>
               [3,5] -> {{item9}}
           </li>  
            <li>
               [3,4] -> {{item10}}
           </li>  
        </ol> 
        <br>
        <span>jumlah swap:10</span> 
    </div>
</template>

<script>
export default {
    data(){
        return {  
            item1: [4,9,7,5,8,9,3], 
            item2: [4,7,9,5,8,9,3],
            item3: [4,7,5,9,8,9,3],
            item4: [4,5,7,9,8,9,3],
            item5: [4,5,7,8,9,9,3],
            item6: [4,5,7,8,9,3,9],
            item7: [4,5,7,8,3,9,9],
            item8: [4,5,7,3,8,9,9],
            item9: [4,5,3,7,8,9,9],
            item10: [4,3,5,7,8,9,9],
            // numbers: [4,9,7,5,8,9,3],
            // items: ''

        }
    },
    created(){  

        // this.sort(this.numbers);

        // for(var i = 0; i < this.numbers.length; i++){
        //     this.items += "," + this.numbers[i];
        // }

        // return this.items.substring(2);
      this.swap1(1,2);
      this.swap2(3,2);
      this.swap3(2,1);
      this.swap4(4,3);
      this.swap5(6,5);
      this.swap6(5,4);
      this.swap7(4,3);
      this.swap8(3,2);
      this.swap9(2,1);
      this.swap10(1,0);
    },
    methods: {

        // swap(arr,x,y){
        //     var temp;
        //     temp = arr[x];
        //     arr[x] = arr[y];
        //     arr[y] = temp;
        // },
        // sort(array){
        //     for(var j=0; j<array.length-1; j++){
        //         for(var k = 1; k<array.length; k++){
        //             if(array[k] < array[k-1]){
        //                 this.swap(array,k,k-1)
        //             }
        //         }
        //     }
        // }


        
        swap1(x, y){ 
            var z = this.item1[y];
            this.item1[y] = this.item1[x];
            this.item1[x] = z;
            return z;
        }, 
         swap2(x, y){ 
            var z = this.item2[y];
            this.item2[y] = this.item2[x];
            this.item2[x] = z;
            return z;
        }, 
         swap3(x, y){ 
            var z = this.item3[y];
            this.item3[y] = this.item3[x];
            this.item3[x] = z;
            return z;
        }, 
         swap4(x, y){ 
            var z = this.item4[y];
            this.item4[y] = this.item4[x];
            this.item4[x] = z;
            return z;
        }, 
         swap5(x, y){ 
            var z = this.item5[y];
            this.item5[y] = this.item5[x];
            this.item5[x] = z;
            return z;
        }, 
         swap6(x, y){ 
            var z = this.item6[y];
            this.item6[y] = this.item6[x];
            this.item6[x] = z;
            return z;
        }, 
         swap7(x, y){ 
            var z = this.item7[y];
            this.item7[y] = this.item7[x];
            this.item7[x] = z;
            return z;
        }, 
         swap8(x, y){ 
            var z = this.item8[y];
            this.item8[y] = this.item8[x];
            this.item8[x] = z;
            return z;
        }, 
         swap9(x, y){ 
            var z = this.item9[y];
            this.item9[y] = this.item9[x];
            this.item9[x] = z;
            return z;
        }, 
         swap10(x, y){ 
            var z = this.item10[y];
            this.item10[y] = this.item10[x];
            this.item10[x] = z;
            return z;
        },    
    }
}
</script>

<style>
div{
    position: relative;
    margin-left: -34em;
}
span{
    margin-left:-7em;
}
 ol {
  word-break: break-all;
  margin: 0;
  padding: 0;
} 
li {
  list-style-position: inside;
  padding: 0;
}
li::before {
  content: "";
  width: 20px;
  display: inline-block;
}
</style>