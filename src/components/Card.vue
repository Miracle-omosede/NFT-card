<template>
    <div class="bg-neutral-cardbg p-5 shadow-xl rounded-lg">
        <!-- card container -->
        <div class="flex">
            <!-- card image -->
                <img src="../assets/images/image-equilibrium.jpg" alt="NFT-image" class="w-60 rounded-lg">
        </div>

        <div class="flex flex-col">
            <!-- all text -->
            <h1 class="text-neutral-white text-lg font-bold pt-5 pb-3">Equilibrum #3329</h1>

            <h6 class="font-medium text-sm text-primary-softblue">Our Equilibrum collection promotes <br>balance and calm.</h6>

            <div class="flex flex-row py-3 justify-between items-center">
                <h6 class="font-bold text-primary-cyan">

                    <!-- Etherium icon -->
                   <fa :icon="['fab', 'ethereum']"/> 
                    {{price}}</h6>
                <h6 class="text-sm font-bold text-primary-softblue">
                    <fa :icon="['fas','clock']" />
                    3 days left </h6>
            </div>

            <!-- divider -->
            <hr class="border-primary-softblue" />

            <div class="flex flex-row items-center pt-4">
                <img src="../assets/images/image-avatar.png" class="w-10  border-white border rounded-full">
                <h6 class=" text-1xs font-light text-neutral-white"> <span class="text-primary-softblue pl-3">Creation of</span>{{creator}}</h6>
            </div>
            <div class="flex justify-center items-center py-3">
              <Button />  
            </div>
        </div>
        <div>
            
        </div>
    </div>
</template>
<script>
import Button from './Button.vue'

export default {
    name: 'Card',
    components : {
        Button
    },
    data() {
        return {
        price: '0.041 ETH ',
        creator: ' Miracle',
        image: '../assets/images/image-avatar.png',
        }
    }
}
</script>

<style scoped>

</style>