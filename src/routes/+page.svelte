<script lang="ts">
let buttons:any = []
const farbe:string = ''
let werte:any = {'intern-downloads':'99BCE3', 'intern-logging':'99BCE3', 'intern-automation':'99BCE3','intern-share':'B7CA9D','intern-namespace':'99BCE3','intern-whoami':'99BCE3','intern-routing':'99BCE3','intern-root':'99BCE3','intern-sec':'99BCE3','extern-engineering':'FAD791','extern-customer':'F2B0A9','extern-playground':'99BCE3','extern-trial':'FBBF93'}

function button_click(input:number){
        for(let button of buttons){
            button.style.display = 'none'
        }
        buttons[input].style.display ='block'
        buttons[input+13].style.display ='block'   
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
    {#each Object.entries(werte) as [rolle_2,farbe],i }
    <tr><td><button on:click={() => button_click(i)}>{rolle_2} </button> </td> <td><button bind:this={buttons[i]}  on:click={() => link(rolle_2,'user',farbe)}   class=invisible>user</button></td><td><button bind:this={buttons[i+ 13]}  on:click={() => link(rolle_2,'chef',farbe)}   class=invisible>chef  </button> </td></tr>
{/each}
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