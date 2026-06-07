<template>
  <div class="app-container">
    <Sidebar :currentSection="currentSection" @navigate="currentSection = $event" />
    <main class="main-content">
      <TopHeader />
      <div v-show="currentSection === 'dashboard'">
        <Dashboard />
      </div>
      <div v-show="currentSection === 'market-research'">
        <MarketResearch />
      </div>
      <div v-show="currentSection === 'innovation-pipeline'">
        <InnovationPipeline />
      </div>
      <div v-show="currentSection === 'risk-assessment'">
        <RiskAssessment />
      </div>
      <div v-show="currentSection === 'benchmarking'">
        <Benchmarking />
      </div>
      <div v-show="currentSection === 'regulatory-watch'">
        <RegulatoryWatch />
      </div>
      <div v-show="currentSection === 'notifications'">
        <Notifications />
      </div>
    </main>
  </div>
</template>

<script setup>
import { ref } from 'vue'
import Sidebar from './components/Sidebar.vue'
import TopHeader from './components/TopHeader.vue'
import Dashboard from './components/Dashboard.vue'
import MarketResearch from './components/MarketResearch.vue'
import InnovationPipeline from './components/InnovationPipeline.vue'
import RiskAssessment from './components/RiskAssessment.vue'
import Benchmarking from './components/Benchmarking.vue'
import RegulatoryWatch from './components/RegulatoryWatch.vue'
import Notifications from './components/Notifications.vue'

import './assets/main.css'

const currentSection = ref('dashboard')
</script>

<style>
.app-container {
  display: flex;
  min-height: 100vh;
}
</style>
