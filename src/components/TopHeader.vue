<template>
                    <header class="header">
                <div class="search-bar">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                        <circle cx="11" cy="11" r="8"></circle>
                        <path d="m21 21-4.35-4.35"></path>
                    </svg>
                    <input type="text" placeholder="Search pipelines, partners, or KPIs..." />
                </div>
                <div class="header-actions" style="gap:20px">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2">
                            <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                            <path d="M13.73 21a2 2 0 0 1-3.46 0"></path>
                        </svg>
                        <span style="position:absolute;top:-4px;right:-6px;width:15px;height:15px;background:#fa0000;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:600;color:#faf8f8">0</span>
                    </div>
                    <div class="user-profile">
                        <div class="avatar" style="border:1px solid #999696"></div>
                        <span class="user-name">Jane Peters</span>
                        <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2">
                            <polyline points="6 9 12 15 18 9"></polyline>
                        </svg>
                    </div>
                    <button class="btn-primary" id="new-brief-btn">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                            <line x1="12" y1="5" x2="12" y2="19"></line>
                            <line x1="5" y1="12" x2="19" y2="12"></line>
                        </svg>
                        New Brief
                    </button>
                </div>
            </header>

</template>
<script setup>
</script>