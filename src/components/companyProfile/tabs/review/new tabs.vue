<template>
<div class="tabsdiv">
          <div class="py-3">
          <ul class="nav nav-tabs tabswesy" role="tablist">
            <li class="ml-2">&nbsp;</li>
            <li class="nav-item">
              <a class="nav-link active newone" id="onenew" data-toggle="tab" href="#newone" role="tab">Owner</a>
            </li>
            <li class="nav-item">
              <a class="nav-link newone" data-toggle="tab" href="#newtwo" role="tab">Opening Times</a>
            </li>
            <li class="nav-item">
              <a class="nav-link newone" data-toggle="tab" href="#newThree" role="tab">Impressume</a>
            </li>
           
          </ul>

          <!-- Tab panes -->
          <div class="tab-content nwtb">
            <div class="tab-pane p-2 active" id="newone" role="tabpanel">
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Ipsa, ullam natus. Nesciunt similique, eos ipsam, voluptate sit blanditiis consequuntur temporibus, beatae obcaecati ut perferendis maxime ratione repellendus magni dolorem quos atque nemo recusandae! Sint consequuntur rem numquam est, maxime animi!
            </div>
            <div class="tab-pane p-2" id="newtwo" role="tabpanel">Lorem ipsum dolor sit amet consectetur adipisicing elit. Maiores, tempore porro! Voluptatibus natus impedit rerum, accusantium alias architecto aperiam rem, nemo iusto quam perspiciatis soluta ex facilis placeat vitae unde eligendi sint. Ea itaque, repellat natus, totam magni, nesciunt quisquam tenetur ipsam iure voluptatum odio perferendis vero fuga. Nemo, dolor.
            </div>
            <div class="tab-pane p-2" id="newThree" role="tabpanel">
              Lorem ipsum dolor sit amet consectetur adipisicing elit. Mollitia repudiandae ab corporis labore expedita atque consequatur quidem eius in saepe officia impedit magni iste sed dolore sint cumque beatae aperiam quia, quasi provident! Beatae animi fuga impedit tenetur, ipsam, cupiditate natus, voluptatum optio quis provident iure labore! Architecto id nesciunt beatae doloribus debitis voluptas, deleniti cumque unde sapiente saepe corrupti! Excepturi, commodi? Maiores voluptates, voluptatem velit doloribus culpa sapiente saepe dicta. Et repellat in, facilis laudantium odio accusantium officiis beatae earum, odit rerum blanditiis quibusdam, libero error adipisci voluptatum porro! Incidunt tempora nisi similique. Saepe minima velit quam repellendus amet.
            </div>
           </div>
        </div>
        </div>
</template>
<script>
// import $ from 'jquery';
// window.$ = $
//  $(document).ready(function() { 
//             $(".newone").click(function() {
//                 $('.newone').css("background-color","white")
//                 $('.newone').css("color","gray")
//                 $(event.target).css("background-color",'rgb(112, 173, 71)') 
//                 $(event.target).css("color",'white') 
//             });  
//         });
export default {
    
}
</script>
<style scoped>
    .nav-tabs .nav-item.show .nav-link,
.nav-tabs .nav-link.active,
.nav-tabs .nav-link.active:hover {
  border-color: #495057 #495057 #fff;
}

.nav-tabs {
  border-bottom-color: #495057;
}

.nav-tabs .nav-link:hover {
  border-color: #ccc #ccc #495057;
  background-color: #eee;
}

.nav-tabs .nav-link.active {
  background-color: rgb(112, 173, 71);
  color: white;
}

.nav-tabs .nav-link {
  margin-right: 4px;
  color:#7a7d7f
}

/* Not essential */

body {
  font-family: "Trebuchet MS";
}

</style>