<script lang="ts">
    
    import { browser } from '$app/environment';
 
function button_click(input:number){
    if (browser) {
        let button1_1:any = document.getElementById('button1_1'),button1_2:any = document.getElementById('button1_2');
        let button2_1:any = document.getElementById('button2_1'),button2_2:any = document.getElementById('button2_2');
        let button3_1:any = document.getElementById('button3_1'),button3_2:any = document.getElementById('button3_2');
        let button4_1:any = document.getElementById('button4_1'),button4_2:any = document.getElementById('button4_2');
        let button5_1:any = document.getElementById('button5_1'),button5_2:any = document.getElementById('button5_2');
        let button6_1:any = document.getElementById('button6_1'),button6_2:any = document.getElementById('button6_2');
        let button7_1:any = document.getElementById('button7_1'),button7_2:any = document.getElementById('button7_2');
        let button8_1:any = document.getElementById('button8_1'),button8_2:any = document.getElementById('button8_2');
        let button9_1:any = document.getElementById('button9_1'),button9_2:any = document.getElementById('button9_2');
        let button10_1:any = document.getElementById('button10_1'),button10_2:any = document.getElementById('button01_2');
        let button11_1:any = document.getElementById('button11_1'),button11_2:any = document.getElementById('button11_2');
        let button12_1:any = document.getElementById('button12_1'),button12_2:any = document.getElementById('button12_2');
        let button13_1:any = document.getElementById('button13_1'),button13_2:any = document.getElementById('button13_2');
        

        
        
    switch(input){
        case 1: 
            button1_1.style.display = 'block'
            button1_2.style.display = 'block'
            break;
        case 2: 
            button2_1.style.display = 'block'
            button2_2.style.display = 'block'
            break;
        case 3: 
            button3_1.style.display = 'block'
            button3_2.style.display = 'block'
            break;
        case 4: 
            button4_1.style.display = 'block'
            button4_2.style.display = 'block'
            break;
        case 5: 
            button5_1.style.display = 'block'
            button5_2.style.display = 'block'
            break;
        case 6: 
            button6_1.style.display = 'block'
            button6_2.style.display = 'block'
            break;
        case 7: 
            button7_1.style.display = 'block'
            button7_2.style.display = 'block'
            break;
        case 8: 
            button8_1.style.display = 'block'
            button8_2.style.display = 'block'
            break;
        case 9: 
            button9_1.style.display = 'block'
            button9_2.style.display = 'block'
            break;
        case 10: 
            button10_1.style.display = 'block'
            button10_2.style.display = 'block'
            break;
        case 11: 
            button11_1.style.display = 'block'
            button11_2.style.display = 'block'
            break;
        case 12: 
            button12_1.style.display = 'block'
            button12_2.style.display = 'block'
            break;
        case 13: 
            button13_1.style.display = 'block'
            button13_2.style.display = 'block'
            break;
        default: 
        alert('hu')
    }
    }
}
</script>


<h1>Rollewechsel</h1>

<div><table>
   <tbody>
        <tr><td><button on:click={() => button_click(1)}>intern-downloads   </button> </td> <td><button class=invisible id= 'button1_1'>user  </button> </td><td><button class=invisible id = 'button1_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(2)}>intern-logging     </button> </td> <td><button class=invisible id= 'button2_1'>user  </button></td><td><button class=invisible id = 'button2_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(3)}>intern-automation  </button> </td> <td><button class=invisible id= 'button3_1'>user  </button> </td><td><button class=invisible id = 'button3_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(4)}>intern-share       </button> </td> <td><button class=invisible id= 'button4_1'>user  </button> </td><td><button class=invisible id = 'button4_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(5)}>intern-namespace   </button> </td> <td><button class=invisible id= 'button5_1'>user  </button> </td><td><button class=invisible id = 'button5_2'>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(6)}>intern-whoami      </button> </td> <td><button class=invisible id= 'button6_1'>user  </button> </td><td><button class=invisible id = 'button6_2'>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(7)}>intern-routing     </button> </td> <td><button class=invisible id= 'button7_1'>user  </button> </td><td><button class=invisible id = 'button7_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(8)}>intern-root        </button> </td> <td><button class=invisible id= 'button8_1'>user  </button> </td><td><button class=invisible id = 'button8_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(9)}>intern-sec         </button> </td> <td><button class=invisible id= 'button9_1'>user  </button> </td><td><button class=invisible id = 'button9_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(10)}>extern-engineering</button> </td> <td><button class=invisible id= 'button10_1'>user  </button> </td><td><button class=invisible id = 'button10_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(11)}>extern-customer   </button> </td> <td><button class=invisible id= 'button11_1'>user  </button> </td><td><button class=invisible id = 'button11_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(12)}>extern-playground </button> </td> <td><button class=invisible id= 'button12_1'>user  </button> </td><td><button class=invisible id = 'button12_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(13)}>extern-trial      </button> </td> <td><button class=invisible id= 'button13_1'>user  </button> </td><td><button class=invisible id = 'button13_2'>chef  </button> </td></tr>
   </tbody>
</table></div>














<style>
div{
    width: max-content;

}
table{
    width: 100%;

}
button{
    height: 100px;
    width:119px;
    margin: 2.5px;
    
}

.invisible{
    display: none;
    
}




</style>





