<template>
<div>

            <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:8px">
                <h1 style="font-size:32px;font-weight:700;color:#2d3643">Overview Dashboard</h1>
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2">
                    <circle cx="12" cy="12" r="10"></circle>
                    <polyline points="12 6 12 12 16 14"></polyline>
                </svg>
            </div>
            <p class="welcome-text">Welcome back Jane, Here's what's happening in your growth pipeline today.</p>
            <div style="display:flex;justify-content:flex-end;gap:12px;margin-bottom:24px">
                <span class="dropdown" style="display:flex;align-items:center;gap:8px;padding:10px 12px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;font-size:16px;font-weight:600;color:#4b5054">
                    Last 30 Days
                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                        <polyline points="6 9 12 15 18 9"></polyline>
                    </svg>
                </span>
                <span class="dropdown" style="display:flex;align-items:center;gap:10px;padding:10px 12px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;font-size:16px;font-weight:600;color:#4b5054">
                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                        <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                        <polyline points="7 10 12 15 17 10"></polyline>
                        <line x1="12" y1="15" x2="12" y2="3"></line>
                    </svg>
                    Export Report
                </span>
            </div>

            <div class="kpi-grid">
                <div class="kpi-card" style="position:relative">
                    <div style="position:absolute;left:22px;top:11px;width:34px;height:36px;background:#f0fdf4;border-radius:4px;display:flex;align-items:center;justify-content:center">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor" style="color:#228b22">
                            <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
                        </svg>
                    </div>
                    <div style="position:absolute;right:21px;top:21px;display:flex;align-items:center;gap:5px;background:#dcfce7;padding:4px 8px;border-radius:8px">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2">
                            <path d="M3 3v18h18"></path>
                            <path d="M18 9l-5 5-4-4-3 3"></path>
                        </svg>
                        <span style="font-size:12px;font-weight:600;color:#228b22">+12.5%</span>
                    </div>
                    <div style="margin-top:60px;font-size:24px;font-weight:600;color:#000">47</div>
                    <div style="font-size:12px;font-weight:600;color:#4b5054;margin-top:4px">RESEARCH BRIEFS</div>
                    <div style="font-size:12px;font-weight:600;color:#4b5054;margin-top:8px;margin-left:35px">Avg. completion: 3.2 days</div>
                </div>
                <div class="kpi-card" style="position:relative">
                    <div style="position:absolute;left:22px;top:11px;width:34px;height:36px;background:#eff6ff;border-radius:4px;display:flex;align-items:center;justify-content:center">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor" style="color:#313eb2">
                            <path d="M3 3v18h18"></path>
                            <path d="M18 9l-5 5-4-4-3 3"></path>
                        </svg>
                    </div>
                    <div style="position:absolute;right:21px;top:21px;display:flex;align-items:center;gap:5px;background:#dcfce7;padding:4px 8px;border-radius:8px">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2">
                            <path d="M3 3v18h18"></path>
                            <path d="M18 9l-5 5-4-4-3 3"></path>
                        </svg>
                        <span style="font-size:12px;font-weight:600;color:#228b22">+12.5%</span>
                    </div>
                    <div style="margin-top:60px;font-size:24px;font-weight:600;color:#000">47</div>
                    <div style="font-size:12px;font-weight:600;color:#4b5054;margin-top:4px">STRATEGY REVIEWS SUPPORTED</div>
                    <div style="font-size:12px;font-weight:600;color:#4b5054;margin-top:8px;margin-left:35px">Data support utilization</div>
                </div>
            </div>

            <div class="charts-grid">
                <div class="chart-card">
                    <div class="chart-header">
                        <div>
                            <div class="chart-title">Innovation Pipeline Funnel</div>
                            <div class="chart-subtitle">Idea flow by stage · Q1 2026</div>
                        </div>
                        <span class="chart-badge badge-blue">23 Ideas</span>
                    </div>
                    <div class="funnel-item">
                        <span class="funnel-label">Idea Log</span>
                        <div class="funnel-bar-container">
                            <div class="funnel-bar" style="width:100%;background:#313eb2"></div>
                        </div>
                        <span class="funnel-count">23</span>
                    </div>
                    <div class="funnel-item">
                        <span class="funnel-label">Scoring</span>
                        <div class="funnel-bar-container">
                            <div class="funnel-bar" style="width:74%;background:#228b22"></div>
                        </div>
                        <span class="funnel-count">17</span>
                    </div>
                    <div class="funnel-item">
                        <span class="funnel-label">Evaluation</span>
                        <div class="funnel-bar-container">
                            <div class="funnel-bar" style="width:57%;background:#ff8d28"></div>
                        </div>
                        <span class="funnel-count">13</span>
                    </div>
                    <div class="funnel-item">
                        <span class="funnel-label">Prototype</span>
                        <div class="funnel-bar-container">
                            <div class="funnel-bar" style="width:26%;background:#eff31c"></div>
                        </div>
                        <span class="funnel-count">6</span>
                    </div>
                    <div class="funnel-item">
                        <span class="funnel-label">Approval</span>
                        <div class="funnel-bar-container">
                            <div class="funnel-bar" style="width:17%;background:#e50303"></div>
                        </div>
                        <span class="funnel-count">4</span>
                    </div>
                </div>
                <div class="chart-card">
                    <div class="chart-header">
                        <div>
                            <div class="chart-title">Risk Severity Heatmap</div>
                            <div class="chart-subtitle">By category × impact level</div>
                        </div>
                        <span class="chart-badge" style="background:#fee2e2;color:#e50303">5 Active</span>
                    </div>
                    <div class="heatmap">
                        <div></div>
                        <div class="heatmap-header">LOW</div>
                        <div class="heatmap-header">MED</div>
                        <div class="heatmap-header">HIGH</div>
                        <div class="heatmap-header">CRITICAL</div>
                        <div class="heatmap-header">SCORE</div>

                        <div class="heatmap-row-label">Regulatory</div>
                        <div class="heatmap-cell positive">2</div>
                        <div class="heatmap-cell positive">3</div>
                        <div class="heatmap-cell positive">1</div>
                        <div class="heatmap-cell positive">2</div>
                        <div class="heatmap-cell" style="background:#fff7ed;color:#ec6c28">4.1</div>

                        <div class="heatmap-row-label">Credit</div>
                        <div class="heatmap-cell positive">2</div>
                        <div class="heatmap-cell warning">2</div>
                        <div class="heatmap-cell critical-light">2</div>
                        <div class="heatmap-cell critical">2</div>
                        <div class="heatmap-cell" style="background:#fef2f2;color:#e71212">7.8</div>

                        <div class="heatmap-row-label">Market</div>
                        <div class="heatmap-cell positive">2</div>
                        <div class="heatmap-cell gray">2</div>
                        <div class="heatmap-cell warning">2</div>
                        <div class="heatmap-cell critical-light">2</div>
                        <div class="heatmap-cell positive">2.4</div>

                        <div class="heatmap-row-label">Compliance</div>
                        <div class="heatmap-cell positive">2</div>
                        <div class="heatmap-cell orange">2</div>
                        <div class="heatmap-cell critical">2</div>
                        <div class="heatmap-cell warning">2</div>
                        <div class="heatmap-cell positive">5.2</div>
                    </div>
                    <div class="legend">
                        <div class="legend-item">
                            <div class="legend-color" style="background:#dcfce7"></div>
                            <span>Low</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background:#fef9c3"></div>
                            <span>Medium</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background:#fed7aa"></div>
                            <span>High</span>
                        </div>
                        <div class="legend-item">
                            <div class="legend-color" style="background:#7f1d1d"></div>
                            <span>Critical</span>
                        </div>
                    </div>
                </div>
                <div class="chart-card" style="padding:0">
                    <div style="padding:16px 16px 0">
                        <div class="chart-title" style="font-size:20px;font-weight:600;color:#000;margin-bottom:17px">Quick Action</div>
                    </div>
                    <div style="padding:0 28px">
                        <div class="quick-actions" style="border:1px solid #e5e5e5;border-radius:4px;padding:9px 15px;margin-bottom:12px">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                                <line x1="12" y1="5" x2="12" y2="19"></line>
                                <line x1="5" y1="12" x2="19" y2="12"></line>
                            </svg>
                            <span class="quick-action-text">Start New Research Brief</span>
                        </div>
                        <div class="quick-actions" style="border:1px solid #e5e5e5;border-radius:4px;padding:9px 15px;margin-bottom:12px">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="currentColor" style="color:#4b5054">
                                <circle cx="12" cy="12" r="10"></circle>
                            </svg>
                            <span class="quick-action-text">Submit Inovation Idea</span>
                        </div>
                        <div class="quick-actions" style="border:1px solid #e5e5e5;border-radius:4px;padding:9px 15px;margin-bottom:12px">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                                <path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"></path>
                            </svg>
                            <span class="quick-action-text">Access Regulatory Watch</span>
                        </div>
                        <div class="quick-actions" style="border:1px solid #e5e5e5;border-radius:4px;padding:9px 15px;margin-bottom:12px">
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2">
                                <path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"></path>
                            </svg>
                            <span class="quick-action-text">View Risk Register</span>
                        </div>
                    </div>
                </div>
            </div>

            <div style="position:relative">
                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2" style="position:absolute;left:184px;top:-30px;z-index:10">
                    <path d="M3 3v18h18"></path>
                    <path d="M18 9l-5 5-4-4-3 3"></path>
                </svg>
                <div class="charts-grid-2">
                    <div class="chart-card">
                        <div class="chart-header">
                            <div>
                                <div class="chart-title">Research Output by Sector</div>
                                <div class="chart-subtitle">Completed briefs · Last 6 months</div>
                            </div>
                            <span class="chart-badge badge-green">+12% MoM</span>
                        </div>
                    </div>
                    <div></div>
                </div>
            </div>

            <div class="activity-section">
                <div class="activity-card">
                    <div class="activity-header">
                        <span class="activity-title">Recent Activity</span>
                        <span style="font-size:12px;color:#0f151f;cursor:pointer">View All</span>
                    </div>
                    <p class="activity-subtitle">Latest submissions & approvals</p>
                    <div class="activity-list">
                        <div class="activity-item">
                            <div>
                                <div class="activity-item-title">Islamic Fintech Landscape Brief</div>
                                <div class="activity-item-meta">Amira Hassan · Market Research</div>
                            </div>
                            <div>
                                <span class="activity-status status-approved">APPROVED</span>
                                <div style="font-size:12px;color:#4b5054;text-align:right">2h ago</div>
                            </div>
                        </div>
                        <div class="activity-item">
                            <div>
                                <div class="activity-item-title">Sukuk Innovation – PE Hybrid Idea</div>
                                <div class="activity-item-meta">Omar Suleiman · Innovation</div>
                            </div>
                            <div>
                                <span class="activity-status status-pending">PENDING</span>
                                <div style="font-size:12px;color:#4b5054;text-align:right">4h ago</div>
                            </div>
                        </div>
                        <div class="activity-item">
                            <div>
                                <div class="activity-item-title">Sukuk Innovation – PE Hybrid Idea</div>
                                <div class="activity-item-meta">Omar Suleiman · Innovation</div>
                            </div>
                            <div>
                                <span class="activity-status status-flagged">FLAGGED</span>
                                <div style="font-size:12px;color:#4b5054;text-align:right">4h ago</div>
                            </div>
                        </div>
                        <div class="activity-item">
                            <div>
                                <div class="activity-item-title">Sukuk Innovation – PE Hybrid Idea</div>
                                <div class="activity-item-meta">Omar Suleiman · Innovation</div>
                            </div>
                            <div>
                                <span class="activity-status status-review">IN REVIEW</span>
                                <div style="font-size:12px;color:#4b5054;text-align:right">4h ago</div>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="table-card">
                    <div class="table-header">
                        <span class="table-title">Active Research Briefs</span>
                        <div class="table-filters">
                            <button class="filter-btn">CSV</button>
                            <button class="filter-btn btn-primary">New</button>
                        </div>
                    </div>
                    <p class="activity-subtitle">47 total · Filtered: All</p>
                    <table class="data-table">
                        <thead>
                            <tr>
                                <th>TITLE</th>
                                <th>ANALYST</th>
                                <th>STATUS</th>
                                <th>ALIGNMENT</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td>Islamic Fintech Landscape</td>
                                <td><span style="display:inline-flex;align-items:center;gap:4px"><span style="width:22px;height:22px;background:#228b22;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;color:#fff;font-size:9px">AH</span> A. Hassan</span></td>
                                <td><span class="activity-status status-approved">Approved</span></td>
                                <td>
                                    <span style="margin-right:8px">92</span>
                                    <div class="alignment-bar" style="display:inline-block;vertical-align:middle"><div class="alignment-fill" style="width:78%"></div></div>
                                </td>
                            </tr>
                            <tr>
                                <td>Islamic Fintech Landscape</td>
                                <td><span style="display:inline-flex;align-items:center;gap:4px"><span style="width:22px;height:22px;background:#313eb2;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;color:#fff;font-size:9px">AH</span> A. Hassan</span></td>
                                <td><span class="activity-status status-pending">Pending</span></td>
                                <td>
                                    <span style="margin-right:8px">92</span>
                                    <div class="alignment-bar" style="display:inline-block;vertical-align:middle"><div class="alignment-fill" style="width:78%"></div></div>
                                </td>
                            </tr>
                            <tr>
                                <td>Islamic Fintech Landscape</td>
                                <td><span style="display:inline-flex;align-items:center;gap:4px"><span style="width:22px;height:22px;background:#0f151f;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;color:#fff;font-size:9px">AH</span> A. Hassan</span></td>
                                <td><span class="activity-status status-review">In review</span></td>
                                <td>
                                    <span style="margin-right:8px">92</span>
                                    <div class="alignment-bar" style="display:inline-block;vertical-align:middle"><div class="alignment-fill" style="width:78%"></div></div>
                                </td>
                            </tr>
                            <tr>
                                <td>Islamic Fintech Landscape</td>
                                <td><span style="display:inline-flex;align-items:center;gap:4px"><span style="width:22px;height:22px;background:#e50303;border-radius:50%;display:inline-flex;align-items:center;justify-content:center;color:#fff;font-size:9px">AH</span> A. Hassan</span></td>
                                <td><span class="activity-status status-approved">Approved</span></td>
                                <td>
                                    <span style="margin-right:8px">92</span>
                                    <div class="alignment-bar" style="display:inline-block;vertical-align:middle"><div class="alignment-fill" style="width:78%"></div></div>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                    <div class="pagination">
                        <span class="pagination-info">Showing 1–5 of 47</span>
                        <div class="pagination-buttons">
                            <button class="page-btn">&lt;</button>
                            <button class="page-btn">1</button>
                            <button class="page-btn">2</button>
                            <button class="page-btn">3</button>
                            <button class="page-btn">...</button>
                            <button class="page-btn">10</button>
                            <button class="page-btn">&gt;</button>
                        </div>
                    </div>
                </div>
            </div>

            <div class="chart-card">
                <div class="chart-header">
                    <div>
                        <span class="chart-title">Executive Summary — Portfolio Contribution by R&D Unit</span>
                        <p style="font-size:12px;color:#4b5054">Aggregated impact · Q1 FY2026</p>
                    </div>
                    <div>
                        <span class="chart-badge badge-green">94% Shari'ah Compliance</span>
                        <span style="margin-left:8px;cursor:pointer">Full Report ↓</span>
                    </div>
                </div>
                <div class="summary-grid">
                    <div class="summary-card">
                        <div class="summary-value">₦4.2B</div>
                        <div class="summary-label">Research-Influenced AUM</div>
                    </div>
                    <div class="summary-card">
                        <div class="summary-value">86%</div>
                        <div class="summary-label">Strategic Alignment</div>
                    </div>
                    <div class="summary-card">
                        <div class="summary-value">98.5%</div>
                        <div class="summary-label">Uptime · Data Refresh</div>
                    </div>
                    <div class="summary-card">
                        <div class="summary-value">14</div>
                        <div class="summary-label">New Products Proposed</div>
                    </div>
                </div>
            </div>


</div>
</template>
<script setup>
import { ref } from "vue";
</script>