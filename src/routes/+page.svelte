<script lang="ts">
let buttons:any = []

function button_click(input:number){
        for(let button of buttons){
            button.style.display = 'none'
        }
        buttons[input].style.display ='block'
        buttons[input+1].style.display ='block'   
}
function link(rolle:string,dienstgrad:string,color:string){
    let splits
    splits =rolle.split('-')
    document.location=`https://signin.aws.amazon.com/switchrole?displayName=${rolle}&roleName=company-${splits[0]}-zone-${splits[1]}-${dienstgrad}&account=company-${splits[0]}-zone-${splits[1]}&color=${color}`;
}
</script>

<h1>Rollewechsel</h1>
<div><table>
   <tbody>
        <tr><td><button on:click={() => button_click(0)}>intern-downloads   </button> </td> <td><button bind:this={buttons[0]}  on:click={() => link('intern-downloads','user','99BCE3')}   class=invisible>user</button></td><td><button bind:this={buttons[1]}  on:click={() => link('intern-downloads','chef','99BCE3')}   class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(2)}>intern-logging     </button> </td> <td><button bind:this={buttons[2]}  on:click={() => link('intern-logging','user','99BCE3')}     class=invisible>user</button></td><td><button bind:this={buttons[3]}  on:click={() => link('intern-logging','chef','99BCE3')}     class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(4)}>intern-automation  </button> </td> <td><button bind:this={buttons[4]}  on:click={() => link('intern-automation','user','99BCE3')}  class=invisible>user</button></td><td><button bind:this={buttons[5]}  on:click={() => link('intern-automation','chef','99BCE3')}  class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(6)}>intern-share       </button> </td> <td><button bind:this={buttons[6]}  on:click={() => link('intern-share','user','B7CA9D')}       class=invisible>user</button></td><td><button bind:this={buttons[7]}  on:click={() => link('intern-share','chef','B7CA9D')}       class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(8)}>intern-namespace   </button> </td> <td><button bind:this={buttons[8]}  on:click={() => link('intern-namespace','user','99BCE3')}   class=invisible>user</button></td><td><button bind:this={buttons[9]}  on:click={() => link('intern-namespace','chef','99BCE3')}   class=invisible>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(10)}>intern-whoami     </button> </td> <td><button bind:this={buttons[10]} on:click={() => link('intern-whoami','user','99BCE3')}      class=invisible>user</button></td><td><button bind:this={buttons[11]} on:click={() => link('intern-whoami','chef','99BCE3')}      class=invisible>chef  </button> </td></tr> 
        <tr><td><button on:click={() => button_click(12)}>intern-routing    </button> </td> <td><button bind:this={buttons[12]} on:click={() => link('intern-routing','user','99BCE3')}     class=invisible>user</button></td><td><button bind:this={buttons[13]} on:click={() => link('intern-routing','chef','99BCE3')}     class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(14)}>intern-root       </button> </td> <td><button bind:this={buttons[14]} on:click={() => link('intern-root','user','99BCE3')}        class=invisible>user</button></td><td><button bind:this={buttons[15]} on:click={() => link('intern-root','chef','99BCE3')}        class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(16)}>intern-sec        </button> </td> <td><button bind:this={buttons[16]} on:click={() => link('intern-sec','user','99BCE3')}         class=invisible>user</button></td><td><button bind:this={buttons[17]} on:click={() => link('intern-sec','chef','99BCE3')}         class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(18)}>extern-engineering</button> </td> <td><button bind:this={buttons[18]} on:click={() => link('extern-engineering','user','FAD791')} class=invisible>user</button></td><td><button bind:this={buttons[19]} on:click={() => link('extern-engineering','chef','FAD791')} class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(20)}>extern-customer   </button> </td> <td><button bind:this={buttons[20]} on:click={() => link('extern-customer','user','F2B0A9')}    class=invisible>user</button></td><td><button bind:this={buttons[21]} on:click={() => link('extern-customer','chef','F2B0A9')}    class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(22)}>extern-playground </button> </td> <td><button bind:this={buttons[22]} on:click={() => link('extern-playground','user','99BCE3')}  class=invisible>user</button></td><td><button bind:this={buttons[23]} on:click={() => link('extern-playground','chef','99BCE3')}  class=invisible>chef  </button> </td></tr>
        <tr><td><button on:click={() => button_click(24)}>extern-trial      </button> </td> <td><button bind:this={buttons[24]} on:click={() => link('extern-trial','user','FBBF93')}       class=invisible>user</button></td><td><button bind:this={buttons[25]} on:click={() => link('extern-trial','chef','FBBF93')}       class=invisible>chef  </button> </td></tr>
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