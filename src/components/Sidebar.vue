<template>
    <aside class="sidebar">
        <div :class="['nav-item', { active: currentSection === 'dashboard' }]" @click="$emit('navigate', 'dashboard')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <rect x="3" y="3" width="7" height="7"></rect>
                <rect x="14" y="3" width="7" height="7"></rect>
                <rect x="14" y="14" width="7" height="7"></rect>
                <rect x="3" y="14" width="7" height="7"></rect>
            </svg>
            Dashboard
        </div>
        <div :class="['nav-item', { active: currentSection === 'market-research' }]" @click="$emit('navigate', 'market-research')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
                <polyline points="14 2 14 8 20 8" fill="none" stroke="currentColor" stroke-width="2"></polyline>
                <path d="M16 13H8" stroke="currentColor" stroke-width="2"></path>
                <path d="M16 17H8" stroke="currentColor" stroke-width="2"></path>
                <path d="M10 9H8" stroke="currentColor" stroke-width="2"></path>
            </svg>
            Market Research
        </div>
        <div :class="['nav-item', { active: currentSection === 'innovation-pipeline' }]" @click="$emit('navigate', 'innovation-pipeline')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M12 2L2 7l10 5 10-5-10-5z"></path>
                <path d="M2 17l10 5 10-5"></path>
                <path d="M2 12l10 5 10-5"></path>
            </svg>
            Innovation Pipeline
        </div>
        <div :class="['nav-item', { active: currentSection === 'risk-assessment' }]" @click="$emit('navigate', 'risk-assessment')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path>
            </svg>
            Risk Assessment
        </div>
        <div :class="['nav-item', { active: currentSection === 'benchmarking' }]" @click="$emit('navigate', 'benchmarking')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <circle cx="12" cy="12" r="10"></circle>
                <circle cx="12" cy="12" r="6"></circle>
                <circle cx="12" cy="12" r="2"></circle>
            </svg>
            Benchmarking
        </div>
        <div :class="['nav-item', { active: currentSection === 'regulatory-watch' }]" @click="$emit('navigate', 'regulatory-watch')" >
            <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                <path d="M18 20V10"></path>
                <path d="M12 20V4"></path>
                <path d="M6 20v-6"></path>
            </svg>
            Regulatory Watch
        </div>
        <div :class="['nav-item', { active: currentSection === 'notifications' }]" @click="$emit('navigate', 'notifications')"  style="margin-top:auto">
            <div style="position:relative;display:inline-flex">
                <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                    <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                    <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
                </svg>
                <span style="position:absolute;top:-2px;right:-4px;width:8px;height:8px;background:#f60101;border-radius:50%"></span>
            </div>
            Notifications
        </div>
    </aside>

</template>
<script setup>
defineProps(['currentSection'])
defineEmits(['navigate'])
</script>