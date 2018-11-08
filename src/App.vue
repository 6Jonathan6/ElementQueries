  <template>
  <div class="min-h-screen bg-grey-darker p-4">
    <div style="width: 420px" class="mx-auto border-l border-r border-dashed border-grey-dark py-4 mb-4">
      <width-dimensions>
        <div slot-scope="{width}" class="profile-card" :class="{'profile-card-horizontal':width>400}">
          <img class="profile-card-image" src="../static/img/toby.jpg" alt="">
          <div class="profile-card-meta">
            <div class="mb-4">
              <p class="text-xl leading-tight">Toby Flenderson</p>
              <p class="text-sm leading-tight text-grey-dark">Human Resources at Dunder Mifflin</p>
            </div>
            <div>
              <button class="btn btn-sm btn-pill btn-indigo-outline">Message</button>
            </div>
          </div>
        </div>
      </width-dimensions>
    </div>
  </div>
</template>
<script>
import WidthDimensions from "@/components/WidthDimensions.vue";
export default {
  name: "app",
  components: { WidthDimensions }
};
</script>

<style src="./assets/css/app.css"/>
