<script lang="ts">
let buttons:any = []
const farbe:string = ''
let werte:any = {'intern-downloads':'99BCE3', 'intern-logging':'99BCE3', 'intern-automation':'99BCE3','intern-share':'B7CA9D','intern-namespace':'99BCE3','intern-whoami':'99BCE3','intern-routing':'99BCE3','intern-root':'99BCE3','intern-sec':'99BCE3','extern-engineering':'FAD791','extern-customer':'F2B0A9','extern-playground':'99BCE3','extern-trial':'FBBF93'}
let dienstgrad_2:string 
let klasse:any =['buttons_class','buttons_class','buttons_class']

function homebutton(){
    for(let button of buttons){
            button.style.display = 'none'
        }  
}
function switch_button_class(i:number){
    klasse =['buttons_class','buttons_class','buttons_class']
    klasse[i] = 'buttons_class_2'
}
function buttons_show(){
    for(let button of buttons){
            button.style.display = 'block'
        }  
        
}
function user_chef(input:string){
    dienstgrad_2 = input
}
function link(rolle:string,dienstgrad:string,color:string){
    let splits
    splits =rolle.split('-')
    document.location=`https://signin.aws.amazon.com/switchrole?displayName=${rolle}&roleName=company-${splits[0]}-zone-${splits[1]}-${dienstgrad}&account=company-${splits[0]}-zone-${splits[1]}&color=${color}`;
}
</script>

<h1>Rollewechsel</h1>
<div class= table_1><table class= table_1>
    <tbody>
    <tr><td><button on:click={() => homebutton()} on:click={() => switch_button_class(0)} class={klasse[0]} >Home</button></td><td> <button class={klasse[1]} on:click={() => user_chef('user')} on:click={() => switch_button_class(1)} on:click={() => buttons_show()}>User</button></td><td><button on:click={() => switch_button_class(2)} class={klasse[2]} on:click={() => user_chef('chef')} on:click={() => buttons_show()}>Chef</button></td>
    </tr>
    </tbody>
</table></div>
<div><table>
    <tbody>
    {#each Object.entries(werte) as [rolle_2,farbe],i }
    <tr><td><button  bind:this ={buttons[i]} on:click={() => link(rolle_2,dienstgrad_2,farbe)} >{rolle_2} </button> </td> </tr>
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
    height: 40px;
    width:119px;
    margin: 1px; 
}
.invisible{
    display: none;   
}
.table_1{
    background-color: rgb(141, 141, 211);
    width:100%;
    display:flex;
}
hr{
    margin-bottom: 10px;
}
.buttons_class{
    background-color:rgb(141, 141, 211);
    border: 0px;
}
.buttons_class_2{
    background-color:white;
    color: rgb(141, 141, 211);
    border: 0px;
}

</style>