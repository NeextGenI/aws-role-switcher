<script lang="ts">
let buttons:any = []
const farbe:string = ''
let werte:any = {'intern-downloads':'99BCE3', 'intern-logging':'99BCE3', 'intern-automation':'99BCE3','intern-share':'B7CA9D','intern-namespace':'99BCE3','intern-whoami':'99BCE3','intern-routing':'99BCE3','intern-root':'99BCE3','intern-sec':'99BCE3','extern-engineering':'FAD791','extern-customer':'F2B0A9','extern-playground':'99BCE3','extern-trial':'FBBF93'}
let dienstgrad_2:string 
let klasse:any =['buttons_class','buttons_class','buttons_class']
let text:string =''
let classe:string ='visible'

function homebutton(){
    for(let button of buttons){
            button.style.display = 'none'
        } 
        classe='visible'

}
function switch_button_class(i:number){
    klasse =['buttons_class','buttons_class','buttons_class']
    klasse[i] = 'buttons_class_2'
    switch(i){
        case 0:
            text = 'This is a program that is intended to make changing roles in aws easier.'
            break;
        case 1:
            text = 'This is the interface if you want to continue as <span style="color:blue"> user</span> in aws.'
            break;
        case 2:
            text = 'This is the interface if you want to continue as <span style="color:blue"> chef</span> in aws.'
    }
}
function buttons_show(){
    for(let button of buttons){
            button.style.display = 'block'
        }  
        
}
function user_chef(input:string){
    dienstgrad_2 = input
    classe='invisible'
}
function link(rolle:string,dienstgrad:string,color:string){
    let splits
    splits =rolle.split('-')
    document.location=`https://signin.aws.amazon.com/switchrole?displayName=${rolle}&roleName=company-${splits[0]}-zone-${splits[1]}-${dienstgrad}&account=company-${splits[0]}-zone-${splits[1]}&color=${color}`;
}

switch_button_class(0)
</script>

<h1>AWS-ROLE-SWITCHER</h1>
<div class= table_1><table class= table_1>
    <tbody>
    <tr><td><button on:click={() => homebutton()} on:click={() => switch_button_class(0)} class={klasse[0]} >Home</button></td><td> <button class={klasse[1]} on:click={() => user_chef('user')} on:click={() => switch_button_class(1)} on:click={() => buttons_show()}>User</button></td><td><button on:click={() => switch_button_class(2)} class={klasse[2]} on:click={() => user_chef('chef')} on:click={() => buttons_show()}>Chef</button></td>
    </tr>
    </tbody>
</table></div>
<div><table>
    <tbody>
    {#each Object.entries(werte) as [rolle_2,farbe],i }
    <tr><td><button  bind:this ={buttons[i]} on:click={() => link(rolle_2,dienstgrad_2,farbe)} class= invisible>{rolle_2} </button> </td> </tr>
    {/each}
   </tbody>
</table></div>
	<p class= right_position>{@html text}</p>
    <h3 class= {classe}>Operation manual</h3>
    <p class= {classe}>
        At first you have to click the user or chef button, depending on which you need.<br> After that there will pop out buttons, which by clicking will open a link to the filled in aws role switch form.
    </p>

<style>
   
div{
    width: max-content;
}
button{
    height: 40px;
    width:119px;
    margin: 1px; 
}
.invisible{
    display: none;   
}
.visible{
    display: block;
    position:relative;
    left: 144px;
   
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
.right_position{
    position: absolute;
    left: 150px;
    top: 130px;
}

</style>