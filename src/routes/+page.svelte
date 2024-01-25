<script lang="ts">

function button_click(input:number){
        let button1_1:any = document.getElementById('button1_1'),button1_2:any = document.getElementById('button1_2');
        let button2_1:any = document.getElementById('button2_1'),button2_2:any = document.getElementById('button2_2');
        let button3_1:any = document.getElementById('button3_1'),button3_2:any = document.getElementById('button3_2');
        let button4_1:any = document.getElementById('button4_1'),button4_2:any = document.getElementById('button4_2');
        let button5_1:any = document.getElementById('button5_1'),button5_2:any = document.getElementById('button5_2');
        let button6_1:any = document.getElementById('button6_1'),button6_2:any = document.getElementById('button6_2');
        let button7_1:any = document.getElementById('button7_1'),button7_2:any = document.getElementById('button7_2');
        let button8_1:any = document.getElementById('button8_1'),button8_2:any = document.getElementById('button8_2');
        let button9_1:any = document.getElementById('button9_1'),button9_2:any = document.getElementById('button9_2');
        let button10_1:any = document.getElementById('button10_1'),button10_2:any = document.getElementById('button10_2');
        let button11_1:any = document.getElementById('button11_1'),button11_2:any = document.getElementById('button11_2');
        let button12_1:any = document.getElementById('button12_1'),button12_2:any = document.getElementById('button12_2');
        let button13_1:any = document.getElementById('button13_1'),button13_2:any = document.getElementById('button13_2');
        
            button1_1.style.display = 'none'
            button1_2.style.display = 'none'
            button2_1.style.display = 'none'
            button2_2.style.display = 'none'
            button3_1.style.display = 'none'
            button3_2.style.display = 'none'
            button4_1.style.display = 'none'
            button4_2.style.display = 'none'
            button5_1.style.display = 'none'
            button5_2.style.display = 'none'
            button6_1.style.display = 'none'
            button6_2.style.display = 'none'
            button7_1.style.display = 'none'
            button7_2.style.display = 'none'
            button8_1.style.display = 'none'
            button8_2.style.display = 'none'
            button9_1.style.display = 'none'
            button9_2.style.display = 'none'
            button10_1.style.display = 'none'
            button10_2.style.display = 'none'
            button11_1.style.display = 'none'
            button11_2.style.display = 'none'
            button12_1.style.display = 'none'
            button12_2.style.display = 'none'
            button13_1.style.display = 'none'
            button13_2.style.display = 'none'

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
function link(input_2:number){
    switch(input_2){
        case 1:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-downloads&roleName=company-intern-zone-downloads-user&account=company-intern-zone-downloads&color=99BCE3"
            break;
        case 2:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-downloads&roleName=company-intern-zone-downloads-chef&account=company-intern-zone-downloads&color=99BCE3"
            break;
        case 3:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-logging&roleName=company-intern-zone-logging-user&account=company-intern-zone-logging&color=99BCE3"
            break;
        case 4:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-logging&roleName=company-intern-zone-logging-chef&account=company-intern-zone-logging&color=99BCE3"
            break;
        case 5:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-automation&roleName=company-intern-zone-automation-user&account=company-intern-zone-automation&color=99BCE3"
            break;
        case 6:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-automation&roleName=company-intern-zone-automation-chef&account=company-intern-zone-automation&color=99BCE3"
            break;
        case 7:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-share&roleName=company-intern-zone-share-user&account=company-intern-zone-share&color=B7CA9D"   
            break;
        case 8:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-share&roleName=company-intern-zone-share-chef&account=company-intern-zone-share&color=B7CA9D"
            break;
        case 9:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-namespace&roleName=company-intern-zone-namespace-user&account=company-intern-zone-namespace&color=99BCE3"
            break;
        case 10:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-namespace&roleName=company-intern-zone-namespace-chef&account=company-intern-zone-namespace&color=99BCE3"
             break;
        case 11:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-namespace&roleName=company-intern-zone-namespace-chef&account=company-intern-zone-namespace&color=99BCE3"
            break;
        case 12:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-whoami&roleName=company-intern-zone-whoami-chef&account=company-intern-zone-whoami&color=99BCE3"
            break;
        case 13:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-routing&roleName=company-intern-zone-routing-user&account=company-intern-zone-routing&color=99BCE3" 
            break;
        case 14:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-routing&roleName=company-intern-zone-routing-chef&account=company-intern-zone-routing&color=99BCE3"
        case 15:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-root&roleName=company-intern-zone-root-user&account=company-intern-zone-root&color=99BCE3"
            break;
        case 16:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-root&roleName=company-intern-zone-root-chef&account=company-intern-zone-root&color=99BCE3"
            break;
        case 17:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-sec&roleName=company-intern-zone-sec-user&account=company-intern-zone-sec&color=99BCE3"
            break;
        case 18:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=intern-sec&roleName=company-intern-zone-sec-chef&account=company-intern-zone-sec&color=99BCE3"
            break;
        case 19:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-engineering&roleName=company-extern-zone-engineering-user&account=company-extern-zone-engineering&color=FAD791"
            break;
        case 20:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-engineering&roleName=company-extern-zone-engineering-chef&account=company-extern-zone-engineering&color=FAD791"
            break;
        case 21:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-customer&roleName=company-extern-zone-customer-user&account=company-extern-zone-customer&color=F2B0A9"
            break;
        case 22:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-customer&roleName=company-extern-zone-customer-chef&account=company-extern-zone-customer&color=F2B0A9"
            break;
        case 23:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-playground&roleName=company-extern-zone-playground-user&account=company-extern-zone-playground&color=99BCE3"
            break;
        case 24:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-playground&roleName=company-extern-zone-playground-chef&account=company-extern-zone-playground&color=99BCE3"
            break;
        case 25:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-trial&roleName=company-extern-zone-trial-user&account=company-extern-zone-trial&color=FBBF93"
            break;
        case 26:
            document.location="https://signin.aws.amazon.com/switchrole?displayName=extern-trial&roleName=company-extern-zone-trial-chef&account=company-extern-zone-trial&color=FBBF93"
            break;
        }

}
</script>


<h1>Rollewechsel</h1>

<div><table>
   <tbody>
        <tr><td><button on:click={() => button_click(1)}>intern-downloads   </button> </td> <td><button on:click={() => link(1)} class=invisible id= 'button1_1'>user  </button> </td><td><button on:click={() => link(2)} class=invisible id = 'button1_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(2)}>intern-logging     </button> </td> <td><button on:click={() => link(3)} class=invisible id= 'button2_1'>user  </button> </td><td><button on:click={() => link(4)} class=invisible id = 'button2_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(3)}>intern-automation  </button> </td> <td><button on:click={() => link(5)} class=invisible id= 'button3_1'>user  </button> </td><td><button on:click={() => link(6)} class=invisible id = 'button3_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(4)}>intern-share       </button> </td> <td><button on:click={() => link(7)} class=invisible id= 'button4_1'>user  </button> </td><td><button on:click={() => link(8)} class=invisible id = 'button4_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(5)}>intern-namespace   </button> </td> <td><button on:click={() => link(9)} class=invisible id= 'button5_1'>user  </button> </td><td><button on:click={() => link(10)} class=invisible id = 'button5_2'>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(6)}>intern-whoami      </button> </td> <td><button on:click={() => link(11)} class=invisible id= 'button6_1'>user  </button> </td><td><button on:click={() => link(12)} class=invisible id = 'button6_2'>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(7)}>intern-routing     </button> </td> <td><button on:click={() => link(13)} class=invisible id= 'button7_1'>user  </button> </td><td><button on:click={() => link(14)} class=invisible id = 'button7_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(8)}>intern-root        </button> </td> <td><button on:click={() => link(15)} class=invisible id= 'button8_1'>user  </button> </td><td><button on:click={() => link(16)} class=invisible id = 'button8_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(9)}>intern-sec         </button> </td> <td><button on:click={() => link(17)} class=invisible id= 'button9_1'>user  </button> </td><td><button on:click={() => link(18)} class=invisible id = 'button9_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(10)}>extern-engineering</button> </td> <td><button on:click={() => link(19)} class=invisible id= 'button10_1'>user  </button> </td><td><button on:click={() => link(20)} class=invisible id = 'button10_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(11)}>extern-customer   </button> </td> <td><button on:click={() => link(21)} class=invisible id= 'button11_1'>user  </button> </td><td><button on:click={() => link(22)} class=invisible id = 'button11_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(12)}>extern-playground </button> </td> <td><button on:click={() => link(23)} class=invisible id= 'button12_1'>user  </button> </td><td><button on:click={() => link(24)} class=invisible id = 'button12_2'>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(13)}>extern-trial      </button> </td> <td><button on:click={() => link(25)} class=invisible id= 'button13_1'>user  </button> </td><td><button on:click={() => link(26)} class=invisible id = 'button13_2'>chef  </button> </td></tr>
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





