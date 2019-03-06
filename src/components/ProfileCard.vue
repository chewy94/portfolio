<template>
  <v-card>
    <v-container>
      <v-layout
        row
        wrap
      >
        <v-flex xs12 md5 class="pr-3">
          <v-img
            style="border-radius: 50%;"
            src="https://avatars0.githubusercontent.com/u/25789424?s=400&u=0980d05a1e23eb957eda46af38f774829cb9df0a&v=4"
          />
        </v-flex>
        <v-flex xs12 md7 text-xs-left>
          <v-layout row wrap>
            <v-flex xs12>
              <v-card-text class="display-1 pb-0">
                <span class="font-weight-light">I'm</span><span class="font-weight-bold"> Sean Kimball</span>
              </v-card-text>
            </v-flex>
            <v-flex xs12>
              <v-card-text class="subheading pt-0">
                Full-stack Developer and Manager
              </v-card-text>
              <v-divider style="margin-left: 15px"/>
            </v-flex>
            <v-flex xs12>
              <v-data-iterator
                :items="[
                  { email: 'smkimbal@gmail.com', phone: '+1 480 462 8557', availability: 'Part-time' }
                ]"
                content-tag="v-layout"
                hide-actions
                row
                wrap
              >
                <template v-slot:item="props">
                  <v-flex xs12 md8>
                    <v-card flat>
                      <v-list dense>
                        <v-list-tile>
                          <v-list-tile-content>Email:</v-list-tile-content>
                          <v-list-tile-content class="align-end">{{ props.item.email }}</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-content>Phone:</v-list-tile-content>
                          <v-list-tile-content class="align-end">{{ props.item.phone }}</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-content>Availability:</v-list-tile-content>
                          <v-list-tile-content class="align-end">{{ props.item.availability }}</v-list-tile-content>
                        </v-list-tile>
                        <v-list-tile>
                          <v-list-tile-content>Coffee Per Day:</v-list-tile-content>
                          <v-list-tile-content class="align-end">
                            <v-chip label color="primary">
                              3 Gal<v-icon class="pl-2">mdi-coffee</v-icon>
                            </v-chip>
                          </v-list-tile-content>
                        </v-list-tile>
                      </v-list>
                    </v-card>
                  </v-flex>
                </template>
              </v-data-iterator>
            </v-flex>
          </v-layout>
        </v-flex>
      </v-layout>
    </v-container>
    <v-divider />
    <v-card-actions class="primary">
        <v-layout>
          <v-flex>
            <v-btn icon class="mx-4">
              <v-icon>mdi-facebook</v-icon>
            </v-btn>
            <v-btn icon class="mx-4">
              <v-icon>mdi-github-circle</v-icon>
            </v-btn>
            <v-btn icon class="mx-4">
              <v-icon>mdi-twitter</v-icon>
            </v-btn>
            <v-btn icon class="mx-4">
              <v-icon>mdi-linkedin</v-icon>
            </v-btn>
          </v-flex>
        </v-layout>
      </v-card-actions>
  </v-card>
</template>

<script>
export default {
  
}
</script>
