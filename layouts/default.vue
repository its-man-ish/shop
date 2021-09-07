<template>
  <v-app dark>
    <v-navigation-drawer
      v-model="drawer"
      :mini-variant="miniVariant"
      :clipped="clipped"
      fixed
      app
    >
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
    <!-- Collection -->
        <v-list-item
          v-for="(c, i) in Lnavs"
          :key="i"
          :to="c.to"
          router
          exact
        >
          <v-list-item-action>
          <v-avatar>
            <img :src="c.img" alt="">
          </v-avatar>
          </v-list-item-action>

          <v-list-item-content>
            <v-list-item-title v-text="c.title" />
          </v-list-item-content>
        </v-list-item>

      </v-list>
    </v-navigation-drawer>
    <v-app-bar
      :clipped-left="clipped"
      fixed
      flat
      class="outline"
      outlined
      app
    >

      <v-btn icon router to="/" class="mx-3 pa-1">
       <v-avatar class="">
         <img src="https://media-exp1.licdn.com/dms/image/C4E0BAQFv8X2vXjB-Zw/company-logo_200_200/0/1599732981061?e=2159024400&v=beta&t=Uc3B4svENyJvAab3cOzC5KXSMjqOX67POYOdbsuqmys"
          alt="">
       </v-avatar>
      </v-btn>
<!-- spacer number one -->
      <v-spacer />
<!-- Search box -->
      <v-autocomplete
      v-model="select"
      :loading="loading"
      :items="items.title"
      :search-input.sync="search"
      cache-items
      class="mx-1 hidden-md-and-down"
      flat
      hide-no-data
      hide-details
      label="Find your look"
      solo-inverted
    ></v-autocomplete>

  <!-- Nav list -->
    <v-item-group class="mx-2">
        <v-item v-for="(nav,i) in Rnavs"  :key="i"
        exact>
         <v-btn icon :to="nav.to">
           <v-icon>{{nav.icon}}</v-icon>
         </v-btn>
        </v-item>
    </v-item-group>


      <v-btn
        icon
        @click.stop="rightDrawer = !rightDrawer"
        colors="warning"

      >
        <v-icon>mdi-shopping</v-icon>
      </v-btn>

      <v-btn icon  @click.stop="drawer = !drawer">

        <v-icon v-if="!drawer">mdi-view-dashboard</v-icon>
        <v-icon v-if="drawer">mdi-close</v-icon>
      </v-btn>


    </v-app-bar>
    <v-main>

        <Nuxt />

    </v-main>
    <v-navigation-drawer
      v-model="rightDrawer"
      :right="right"
      temporary
      fixed
    >
      <v-list>
        <v-list-item @click.native="right = !right">
          <v-list-item-action>
            <v-icon light>
              mdi-repeat
            </v-icon>
          </v-list-item-action>
          <v-list-item-title>Switch drawer (click me)</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-navigation-drawer>
    <v-footer
      :absolute="!fixed"
      app
    >
      <span>&copy; {{ new Date().getFullYear() }}</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      Lnavs:[
        {
          img:"https://www.bucco.us/wp-content/uploads/2021/05/Summer-Mens-Wear.jpg",
          title:"MEN",
          to:"/shop/men"
        },
        {
          img:"https://m.media-amazon.com/images/I/61KpUWfdFfL._UX569_.jpg",
          title:"WOMEN",
          to:"/shop/women"
        },
        {
          img:"https://4.imimg.com/data4/NW/TW/MY-25800967/kids-wear-500x500.jpg",
          title:"KIDS",
          to:"/shop/kids"
        },
      ],
      Rnavs:[

        {
          icon:"mdi-account",
          title:"Profile",
          to:"/my-account"
        },
      ],


      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Categaries',
          to: '/Categaries'
        },

      ],
      select:null,
      search:null,
      loading: false,
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'YellowBacks'
    }
  }
}
</script>
