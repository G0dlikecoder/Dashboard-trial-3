<template>
  
  <v-app>
     <v-layout row>
         <v-flex md2>
      <div>
        <v-layout>
          <v-img src="https://alchemy-research.com/wp-content/uploads/2015/08/Background-Design-Theme-Light-Gray.jpg" height="170">
          <v-avatar size="99" class="ma-3">
                 <v-img src="./me2.jpg"></v-img>
          </v-avatar>
            <p class="ma-3">Susas U.</p>
         </v-img>
       </v-layout>
    
         </div>
         <v-card class="mx-auto"
    max-width="600"
    height="670"
    tile>
        
           <v-list>
        <v-list-item
          v-for="(item, i) in items"
          :key="i"
          :to="item.to"
          router
          exact
        >
          <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title v-text="item.title" />
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-divider />
        
      
     <v-col> <p class="mt-6 ml-6 font-weight-black">Unikwan<span class="ml-1 font-weight-black">&copy;</span></p>
     <p>
       <span class=" ml-6 primary--text font-weight-black">Privacy</span> <span class="font-weight-black" >&</span> <span class="primary--text font-weight-black">Terms</span></p></v-col>
         </v-card>
         </v-flex>
         <v-flex md></v-flex>
        <v-flex md6></v-flex>
        <v-flex md></v-flex>
        <v-flex md2>
          <div>
             <v-container class="grey lighten-4">
               <v-layout>
                 <v-col>
                   <p class="font-weight-black">
                   New Message
                 </p>
                     <v-row
              align="center"
              class="spacer ma-5"
              no-gutters>
              <v-avatar>
                           <img
                             src="http://aux.iconspalace.com/uploads/117428211619219278.png"
                             alt="John"
                           >
                         </v-avatar>
                            
                              <p class="ml-5 mt-2 font-weight-regular">Von dan
                              <br/>
                               3 hours ago</p>
                             </v-row>
              <v-row
              align="center"
              class="spacer ma-5"
              no-gutters>
              <v-avatar>
                  <img
                  src="https://www.pngkey.com/png/detail/314-3148038_cartoon-faces-anime-naruto-kakashi-naruto-shippuden-hatake.png"
                             alt="John"
                           >
                         </v-avatar>
                            <p class="ml-5 mt-2 font-weight-regular">Micky
                              <br/>
                               2 hours ago</p>
              </v-row>
              <v-row
              align="center"
              class="spacer ma-5"
              no-gutters>
                <v-avatar>
                    <img
                     src="http://img06.deviantart.net/419b/i/2013/255/e/a/ahri_chibi_by_k_waii-d6m0jrr.png"
                      alt="John"
                    >
                 </v-avatar>
                   <p class="ml-5 mt-2 font-weight-regular">Loren
                      <br/>
                       3 hours ago</p>
              </v-row>
              <p class="font-weight-black">EVENTS</p>
              <p class="font-weight-medium">Team Scrum</p>
              <v-divider></v-divider>
              <p class="font-weight-medium">Google I/O</p>
              <v-divider></v-divider>
              <p class="font-weight-light">No more events scheduled</p>
              <v-divider></v-divider>
              <p class="mt-5">Stats</p>
              <v-img src="https://www.pngkey.com/png/detail/243-2438293_stats-chart-outdoor-setting-top-view.png">

              </v-img>
                 </v-col>
                 
            
                 
               </v-layout>
              </v-container>
         </div>
        </v-flex>
       </v-layout>
      </v-app>
</template>

<script>
export default {
  data () {
    return {
      
      drawer: true,
     
      items: [
        {
          icon: 'mdi-apps',
          title: 'Dashboard',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Projects',
          to: '/Projects'
        },
        {
          icon: 'mdi-watch',
          title: 'Leaderboard',
          to: '/Leaderboard'
        },
        {
          icon: 'mdi-mouse ',
          title: 'Sales',
          to: '/Sales'
        },
        {
          icon: 'mdi-pin',
          title: 'Reports',
          to: '/Reports'
        },
        {
          icon: 'mdi-folder',
          title: 'Statements',
          to: '/Statements'
        },
        {
          icon: 'mdi-archive',
          title: 'Analytics',
          to: '/Analytics'
        },
        {
          icon: 'mdi-anchor',
          title: 'Expenses',
          to: '/Expenses'
        },
        {
          icon: 'mdi-xbox-controller',
          title: 'User',
          to: '/user'
        }
      ],
      
      
    }
  }
}
</script>
