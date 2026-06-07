<template>
<div>
            <div style="display:flex;align-items:center;justify-content:space-between;background:#fff;padding:16px 24px;border-radius:12px;margin-bottom:24px">
                <h1 style="font-size:24px;font-weight:700;color:#2d3643">Notifications</h1>
                <div style="display:flex;align-items:center;gap:16px">
                    <div style="position:relative;display:inline-flex">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                        <span style="position:absolute;top:-4px;right:-6px;width:15px;height:15px;background:#fa0000;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:10px;font-weight:600;color:#faf8f8">3</span>
                    </div>
                    <button style="display:flex;align-items:center;gap:8px;background:#228b22;color:#fff;padding:10px 16px;border-radius:8px;font-weight:600;font-size:16px;border:none;cursor:pointer">Mark All Read</button>
                </div>
            </div>
            <div style="background:#fff;border-radius:12px;overflow:hidden">
                <div style="display:flex;align-items:center;gap:12px;padding:16px 24px;border-bottom:1px solid #e5e5e5;opacity:1">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                        <span style="position:absolute;top:-2px;right:-4px;width:8px;height:8px;background:#f60101;border-radius:50%"></span>
                    </div>
                    <div style="flex:1">
                        <div style="font-size:16px;font-weight:600;color:#000">Research Brief Approved</div>
                        <div style="font-size:14px;color:#4b5054">Islamic Fintech Landscape brief has been approved by the review committee.</div>
                        <div style="font-size:12px;color:#4b5054;margin-top:4px">2 hours ago</div>
                    </div>
                    <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">NEW</span>
                </div>
                <div style="display:flex;align-items:center;gap:12px;padding:16px 24px;border-bottom:1px solid #e5e5e5;opacity:1">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                        <span style="position:absolute;top:-2px;right:-4px;width:8px;height:8px;background:#f60101;border-radius:50%"></span>
                    </div>
                    <div style="flex:1">
                        <div style="font-size:16px;font-weight:600;color:#000">New Risk Flagged</div>
                        <div style="font-size:14px;color:#4b5054">High severity risk detected in Global Tech Solutions portfolio.</div>
                        <div style="font-size:12px;color:#4b5054;margin-top:4px">5 hours ago</div>
                    </div>
                    <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">NEW</span>
                </div>
                <div style="display:flex;align-items:center;gap:12px;padding:16px 24px;border-bottom:1px solid #e5e5e5;opacity:0.7">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                    </div>
                    <div style="flex:1">
                        <div style="font-size:16px;font-weight:600;color:#000">Innovation Pipeline Update</div>
                        <div style="font-size:14px;color:#4b5054">Healthcare Innovation PE Fund moved to Evaluation stage.</div>
                        <div style="font-size:12px;color:#4b5054;margin-top:4px">1 day ago</div>
                    </div>
                </div>
                <div style="display:flex;align-items:center;gap:12px;padding:16px 24px;border-bottom:1px solid #e5e5e5;opacity:0.7">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                    </div>
                    <div style="flex:1">
                        <div style="font-size:16px;font-weight:600;color:#000">Regulatory Policy Update</div>
                        <div style="font-size:14px;color:#4b5054">New capital requirements issued by Central Bank - review needed.</div>
                        <div style="font-size:12px;color:#4b5054;margin-top:4px">2 days ago</div>
                    </div>
                </div>
                <div style="display:flex;align-items:center;gap:12px;padding:16px 24px;opacity:0.7">
                    <div style="position:relative">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                    </div>
                    <div style="flex:1">
                        <div style="font-size:16px;font-weight:600;color:#000">Benchmark Data Updated</div>
                        <div style="font-size:14px;color:#4b5054">New peer fund data added to Competitive Benchmarking module.</div>
                        <div style="font-size:12px;color:#4b5054;margin-top:4px">3 days ago</div>
                    </div>
                </div>
            </div>
        </div>


    <div id="ip-detail-modal" class="ip-detail-modal">
        <div class="ip-detail-content">
            <div class="ip-detail-header">
                <div style="display:flex;justify-content:space-between;align-items:flex-start">
                    <div style="display:flex;flex-direction:column;gap:8px;flex:1;min-width:0">
                        <div style="display:flex;align-items:center;gap:12px;flex-wrap:wrap">
                            <h2 style="font-size:24px;font-weight:700;color:#000">Shari'ah-Compliant Green Energy Fund</h2>
                            <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:12px;font-size:13px;font-weight:600;background:#fef9c3;color:#946325">In progress</span>
                            <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:12px;font-size:13px;font-weight:600;background:#dcfce7;color:#228b22">Ethical Fund</span>
                        </div>
                        <div style="display:flex;align-items:center;gap:20px;font-size:14px;color:#4b5054;flex-wrap:wrap">
                            <span><strong style="color:#000">Author:</strong> Ahmad Hassan</span>
                            <span><strong style="color:#000">Date:</strong> 1/12/2026</span>
                            <span><strong style="color:#000">Stage:</strong> <span style="color:#228b22;font-weight:600">Evaluation</span></span>
                        </div>
                    </div>
                    <div style="display:flex;align-items:center;gap:12px;flex-shrink:0">
                        <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                            Export PDF
                        </button>
                        <button class="modal-close" @click="closeIpDetail()" style="font-size:32px;line-height:1">&times;</button>
                    </div>
                </div>
            </div>
            <div style="display:flex;border-bottom:1px solid #e5e5e5;background:#fff;padding:0 32px;gap:0;flex-shrink:0">
                <button class="ip-tab-btn active" data-ip-detail-tab="overview" @click="switchIpDetailTab('overview')">Overview</button>
                <button class="ip-tab-btn" data-ip-detail-tab="scoring" @click="switchIpDetailTab('scoring')">Evaluation & Scoring</button>
                <button class="ip-tab-btn" data-ip-detail-tab="timeline" @click="switchIpDetailTab('timeline')">Timeline & Progress</button>
                <button class="ip-tab-btn" data-ip-detail-tab="risk" @click="switchIpDetailTab('risk')">Risk Management</button>
            </div>
            <div class="ip-detail-body">
                <div class="ip-detail-left">
                    <div id="ip-detail-overview" class="ip-detail-panel active">
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <h3 style="font-size:18px;font-weight:700;color:#000;margin-bottom:12px">Idea Description</h3>
                            <p style="font-size:15px;color:#2d3643;line-height:1.7">The fund invests in renewable energy projects while adhering to Islamic finance principles, with a primary focus on solar, wind, and hydroelectric projects in emerging markets. Utilizing Islamic investment structures such as Mudarabah and Musharakah, the fund aims to deliver sustainable returns while promoting ethical investing and Shari'ah compliance. The initiative targets community-owned energy projects across Southeast Asia, the Middle East, and North Africa, combining environmental sustainability with faith-based financial principles.</p>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <h3 style="font-size:18px;font-weight:700;color:#000;margin-bottom:16px">Supporting Documents</h3>
                            <div style="display:flex;align-items:center;gap:12px;background:#d9d9d9;border-radius:8px;padding:14px 16px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                <div style="flex:1"><div style="font-size:15px;font-weight:600;color:#000">Market Analysis Report.pdf</div><div style="font-size:13px;color:#4b5054">2.4 MB</div></div>
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                            </div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <h3 style="font-size:18px;font-weight:700;color:#000;margin-bottom:12px">Related Links & Resources</h3>
                            <div style="display:flex;flex-direction:column;gap:8px">
                                <a href="#" style="color:#228b22;font-size:14px;text-decoration:none">Islamic Finance Guidelines — AAOIFI Standards</a>
                                <a href="#" style="color:#228b22;font-size:14px;text-decoration:none">IRENA — Renewable Energy Market Analysis 2025</a>
                                <a href="#" style="color:#228b22;font-size:14px;text-decoration:none">World Bank — ESG Framework for Emerging Markets</a>
                            </div>
                        </div>
                    </div>
                    <div id="ip-detail-scoring" class="ip-detail-panel">
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <h3 style="font-size:18px;font-weight:700;color:#000;margin-bottom:16px">Evaluation Criteria Breakdown</h3>
                            <div style="display:flex;flex-direction:column;gap:16px">
                                <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Market Potential</span><span style="color:#228b22;font-weight:600">85%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:85%;background:#228b22;border-radius:12px"></div></div></div>
                                <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Shari'ah Compliance</span><span style="color:#228b22;font-weight:600">95%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:95%;background:#228b22;border-radius:12px"></div></div></div>
                                <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Financial Viability</span><span style="color:#228b22;font-weight:600">78%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:78%;background:#228b22;border-radius:12px"></div></div></div>
                                <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Innovation & Impact</span><span style="color:#228b22;font-weight:600">82%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:82%;background:#228b22;border-radius:12px"></div></div></div>
                                <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Risk Assessment</span><span style="color:#ca8a04;font-weight:600">65%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:65%;background:#ca8a04;border-radius:12px"></div></div></div>
                            </div>
                        </div>
                    </div>
                    <div id="ip-detail-timeline" class="ip-detail-panel">
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <h3 style="font-size:18px;font-weight:700;color:#000;margin-bottom:16px">Progress Timeline</h3>
                            <div style="display:flex;flex-direction:column;gap:16px">
                                <div style="display:flex;align-items:flex-start;gap:12px">
                                    <div style="width:28px;height:28px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#fff;font-size:12px">&#10003;</div>
                                    <div><div style="font-size:15px;font-weight:600;color:#000">Idea Submitted</div><div style="font-size:13px;color:#4b5054">Ahmad Hassan · Dec 15, 2025</div></div>
                                </div>
                                <div style="display:flex;align-items:flex-start;gap:12px">
                                    <div style="width:28px;height:28px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#fff;font-size:12px">&#10003;</div>
                                    <div><div style="font-size:15px;font-weight:600;color:#000">Scoring Completed</div><div style="font-size:13px;color:#4b5054">Review Committee · Dec 28, 2025</div></div>
                                </div>
                                <div style="display:flex;align-items:flex-start;gap:12px">
                                    <div style="width:28px;height:28px;border-radius:50%;background:#fef9c3;border:2px solid #ca8a04;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#ca8a04;font-size:12px;font-weight:700;">3</div>
                                    <div><div style="font-size:15px;font-weight:600;color:#000">Evaluation (Current)</div><div style="font-size:13px;color:#4b5054">Started Jan 5, 2026 · Due Feb 5, 2026</div></div>
                                </div>
                                <div style="display:flex;align-items:flex-start;gap:12px">
                                    <div style="width:28px;height:28px;border-radius:50%;background:#e5e5e5;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#999;font-size:12px">4</div>
                                    <div><div style="font-size:15px;font-weight:600;color:#999">Approval</div><div style="font-size:13px;color:#999">Pending evaluation completion</div></div>
                                </div>
                                <div style="display:flex;align-items:flex-start;gap:12px">
                                    <div style="width:28px;height:28px;border-radius:50%;background:#e5e5e5;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#999;font-size:12px">5</div>
                                    <div><div style="font-size:15px;font-weight:600;color:#999">Implementation</div><div style="font-size:13px;color:#999">Pending approval</div></div>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div id="ip-detail-risk" class="ip-detail-panel">
                        <div style="background:#fff;border-radius:12px;padding:20px 24px">
                            <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:16px">
                                <h3 style="font-size:18px;font-weight:700;color:#000;margin:0">Risk Register</h3>
                                <button id="ip-log-risk-btn" style="display:flex;align-items:center;gap:8px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:10px 18px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                                    Log New Risk
                                </button>
                            </div>
                            <div style="overflow-x:auto">
                                <table style="width:100%;border-collapse:collapse;font-size:14px">
                                    <thead>
                                        <tr style="background:#f9fafb;border-bottom:1px solid #e5e5e5">
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Risk ID</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Threat Type</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Description</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Severity</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Status</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Target Resolution</th>
                                            <th style="padding:10px 12px;text-align:left;font-weight:600;color:#4b5054">Owner</th>
                                        </tr>
                                    </thead>
                                    <tbody>
                                        <tr style="border-bottom:1px solid #f0f0f0">
                                            <td style="padding:10px 12px;color:#228b22;font-weight:600">RISK-001</td>
                                            <td style="padding:10px 12px;color:#000">Regulatory / Compliance</td>
                                            <td style="padding:10px 12px;color:#4b5054;max-width:200px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap">Shari'ah governance framework misalignment across jurisdictions</td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fee2e2;color:#dc2626">7.5/10</span></td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fef9c3;color:#946325">Open</span></td>
                                            <td style="padding:10px 12px;color:#4b5054">15/06/2026</td>
                                            <td style="padding:10px 12px;color:#000">Fatima Al-Rashid</td>
                                        </tr>
                                        <tr style="border-bottom:1px solid #f0f0f0">
                                            <td style="padding:10px 12px;color:#228b22;font-weight:600">RISK-002</td>
                                            <td style="padding:10px 12px;color:#000">Market</td>
                                            <td style="padding:10px 12px;color:#4b5054;max-width:200px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap">Currency fluctuation in emerging market energy investments</td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fef9c3;color:#ca8a04">5.0/10</span></td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Mitigated</span></td>
                                            <td style="padding:10px 12px;color:#4b5054">30/07/2026</td>
                                            <td style="padding:10px 12px;color:#000">Omar Khayyam</td>
                                        </tr>
                                        <tr>
                                            <td style="padding:10px 12px;color:#228b22;font-weight:600">RISK-003</td>
                                            <td style="padding:10px 12px;color:#000">Operational</td>
                                            <td style="padding:10px 12px;color:#4b5054;max-width:200px;overflow:hidden;text-overflow:ellipsis;white-space:nowrap">Vendor due diligence gaps in solar panel supply chain</td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fee2e2;color:#dc2626">8.0/10</span></td>
                                            <td style="padding:10px 12px"><span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fef9c3;color:#946325">In Progress</span></td>
                                            <td style="padding:10px 12px;color:#4b5054">01/09/2026</td>
                                            <td style="padding:10px 12px;color:#000">Layla bint Hassan</td>
                                        </tr>
                                    </tbody>
                                </table>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="ip-detail-right">
                    <div style="background:#fff;border-radius:12px;padding:20px">
                        <h3 style="font-size:16px;font-weight:700;color:#000;margin-bottom:16px">Key Metrics</h3>
                        <div style="display:flex;flex-direction:column;gap:14px">
                            <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">Overall Score</span><span style="font-weight:700;color:#228b22">80%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:80%;background:#228b22;border-radius:12px"></div></div></div>
                            <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">Viability</span><span style="font-weight:700;color:#228b22">80%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:80%;background:#228b22;border-radius:12px"></div></div></div>
                            <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">Innovation</span><span style="font-weight:700;color:#228b22">80%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:80%;background:#228b22;border-radius:12px"></div></div></div>
                            <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">Risk Level</span><span style="font-weight:700;color:#e50303">65%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:65%;background:#e50303;border-radius:12px"></div></div></div>
                        </div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:20px">
                        <h3 style="font-size:16px;font-weight:700;color:#000;margin-bottom:12px">Actions</h3>
                        <div style="display:flex;flex-direction:column;gap:8px">
                            <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:10px;background:#228b22;color:#fff;border:none;border-radius:8px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
                                Move to Next Stage
                            </button>
                            <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:10px;background:#fff;color:#e50303;border:1px solid #e50303;border-radius:8px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>
                                Reject Idea
                            </button>
                            <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:10px;background:#fff;color:#000;border:1px solid #e5e5e5;border-radius:8px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>
                                Edit Details
                            </button>
                        </div>
                    </div>
                    <div style="background:#228b22;border-radius:12px;padding:16px 20px;display:flex;align-items:center;gap:10px">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#fff" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                        <div><div style="font-size:16px;font-weight:700;color:#fff">Shari'ah Compliant — Verified</div><div style="font-size:12px;color:#fff;opacity:0.9">Passed compliance screening</div></div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <div id="ip-new-idea-modal" class="modal-overlay">
        <div class="modal-content" style="width:720px;max-height:90vh;display:flex;flex-direction:column">
            <div class="modal-header">
                <div class="modal-title">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>
                    Submit New Innovation Idea
                </div>
                <button class="modal-close" @click="closeIpNewIdeaModal()">&times;</button>
            </div>
            <div class="modal-divider"></div>
            <div style="padding:24px 32px 0;display:flex;align-items:center;gap:0">
                <div style="display:flex;align-items:center;gap:8px;flex:1">
                    <div id="ip-step-1-indicator" style="width:36px;height:36px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;color:#fff;font-size:14px;font-weight:700;flex-shrink:0">1</div>
                    <div><div style="font-size:13px;color:#4b5054">Step 1</div><div style="font-size:15px;font-weight:600;color:#000">Basic Information</div></div>
                </div>
                <div style="flex:0.5;height:2px;background:#228b22;margin:0 8px"></div>
                <div style="display:flex;align-items:center;gap:8px;flex:1">
                    <div id="ip-step-2-indicator" style="width:36px;height:36px;border-radius:50%;background:#d9d9d9;display:flex;align-items:center;justify-content:center;color:#999;font-size:14px;font-weight:700;flex-shrink:0">2</div>
                    <div><div style="font-size:13px;color:#4b5054">Step 2</div><div style="font-size:15px;font-weight:600;color:#4b5054">Scoring Matrix</div></div>
                </div>
                <div style="flex:0.5;height:2px;background:#d9d9d9;margin:0 8px"></div>
                <div style="display:flex;align-items:center;gap:8px;flex:1">
                    <div id="ip-step-3-indicator" style="width:36px;height:36px;border-radius:50%;background:#d9d9d9;display:flex;align-items:center;justify-content:center;color:#999;font-size:14px;font-weight:700;flex-shrink:0">3</div>
                    <div><div style="font-size:13px;color:#4b5054">Step 3</div><div style="font-size:15px;font-weight:600;color:#4b5054">Attachments & Links</div></div>
                </div>
            </div>
            <div class="modal-body" style="padding:20px 32px 16px;flex:1;overflow-y:auto">
                <div id="ip-new-idea-step-1" class="ip-detail-panel active">
                    <div class="form-group" style="margin-bottom:20px">
                        <label class="form-label-figma">Idea Title <span class="required-figma">*</span></label>
                        <input type="text" class="form-input-figma" placeholder="Enter a clear and concise title" style="height:44px" />
                    </div>
                    <div class="form-group" style="margin-bottom:20px">
                        <label class="form-label-figma">Description <span class="required-figma">*</span></label>
                        <textarea class="form-input-figma form-textarea-figma" placeholder="Enter full description" style="height:140px;min-height:140px"></textarea>
                        <div style="font-size:13px;color:#4b5054;margin-top:4px;text-align:right">0/200 characters</div>
                    </div>
                    <div class="form-group" style="margin-bottom:8px">
                        <label class="form-label-figma">Fund Type <span class="required-figma">*</span></label>
                        <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:10px;margin-top:8px">
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #228b22;border-radius:8px;background:#f6fef6;font-size:14px;font-weight:600;color:#228b22;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                            <div style="display:flex;align-items:center;justify-content:center;padding:12px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:500;color:#4b5054;cursor:pointer">Private Equity</div>
                        </div>
                    </div>
                </div>
                <div id="ip-new-idea-step-2" class="ip-detail-panel">
                    <p style="font-size:14px;color:#4b5054;margin-bottom:16px">Rate your idea across the following criteria</p>
                    <div style="display:flex;flex-direction:column;gap:20px">
                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:6px"><span style="font-weight:600;color:#000">Market Potential</span><span style="color:#228b22;font-weight:600">--</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:0%;background:#228b22;border-radius:12px"></div></div></div>
                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:6px"><span style="font-weight:600;color:#000">Shari'ah Compliance</span><span style="color:#228b22;font-weight:600">--</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:0%;background:#228b22;border-radius:12px"></div></div></div>
                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:6px"><span style="font-weight:600;color:#000">Financial Viability</span><span style="color:#228b22;font-weight:600">--</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:0%;background:#228b22;border-radius:12px"></div></div></div>
                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:6px"><span style="font-weight:600;color:#000">Innovation & Impact</span><span style="color:#228b22;font-weight:600">--</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:0%;background:#228b22;border-radius:12px"></div></div></div>
                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:6px"><span style="font-weight:600;color:#000">Risk Assessment</span><span style="color:#ca8a04;font-weight:600">--</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:0%;background:#ca8a04;border-radius:12px"></div></div></div>
                    </div>
                    <div style="margin-top:20px;padding:16px;background:#f9fafb;border-radius:8px;display:flex;align-items:center;justify-content:space-between">
                        <span style="font-size:14px;font-weight:600;color:#000">Overall Score</span>
                        <span style="font-size:20px;font-weight:700;color:#4b5054">--</span>
                    </div>
                </div>
                <div id="ip-new-idea-step-3" class="ip-detail-panel">
                    <div class="form-group" style="margin-bottom:20px">
                        <label class="form-label-figma">Supporting Documents</label>
                        <div class="form-upload-figma" style="border:1.5px dashed #e5e5e5;border-radius:8px;padding:32px 16px;text-align:center;cursor:pointer">
                            <svg width="40" height="40" viewBox="0 0 24 24" fill="none" stroke="#667085" stroke-width="2" style="display:block;margin:0 auto 8px"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                            <span style="font-size:14px;color:#000">Drag & drop files or <strong style="color:#228b22">browse</strong></span>
                            <div style="font-size:12px;color:#4b5054;margin-top:4px">PDF, XLSX, DOCX, CSV &middot; Max 25MB per file</div>
                        </div>
                    </div>
                    <div class="form-group" style="margin-bottom:8px">
                        <label class="form-label-figma">Related Links</label>
                        <input type="text" class="form-input-figma" placeholder="https://" style="height:44px;margin-bottom:10px" />
                        <input type="text" class="form-input-figma" placeholder="https://" style="height:44px;margin-bottom:10px" />
                        <input type="text" class="form-input-figma" placeholder="https://" style="height:44px" />
                        <div style="font-size:13px;color:#228b22;margin-top:6px;cursor:pointer">+ Add another link</div>
                    </div>
                </div>
            </div>
            <div class="modal-footer-figma" style="display:flex;justify-content:space-between;align-items:center;padding:0 32px 24px">
                <button id="ip-save-draft-btn" class="btn-modal-figma btn-modal-cancel" style="display:flex;align-items:center;gap:8px">
                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                    Save Draft
                </button>
                <div style="display:flex;gap:12px">
                    <button id="ip-prev-step-btn" class="btn-modal-figma btn-modal-cancel" style="display:none">
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                        Previous
                    </button>
                    <button id="ip-next-step-btn" class="btn-modal-figma btn-modal-submit" style="display:flex;align-items:center;gap:8px">
                        Next Step
                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="9 18 15 12 9 6"/></svg>
                    </button>
                </div>
            </div>
        </div>
    </div>

    <div id="ip-log-risk-modal" class="modal-overlay" style="z-index:1100">
        <div class="modal-content" style="width:680px;max-height:90vh;display:flex;flex-direction:column;background:#f5f5f5">
            <div class="modal-header" style="background:#fff;border-radius:16px 16px 0 0">
                <div class="modal-title" style="font-size:20px;font-weight:700;color:#000">Log New Risk</div>
                <button class="modal-close" @click="closeIpLogRiskModal()">&times;</button>
            </div>
            <div class="modal-body" style="padding:24px 32px;flex:1;overflow-y:auto;background:#f5f5f5">
                <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:20px">
                    <div class="form-group">
                        <label class="form-label-figma">Linked Proposal/Idea <span class="required-figma">*</span></label>
                        <div style="position:relative">
                            <select class="form-input-figma form-select-figma" style="height:44px;appearance:none;padding-right:40px;width:100%;background:#fff">
                                <option>Select Proposal</option>
                                <option>Shari'ah-Compliant Green Energy Fund</option>
                                <option>Islamic Microfinance Sukuk</option>
                                <option>Halal Supply Chain REIT</option>
                            </select>
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="position:absolute;right:12px;top:50%;transform:translateY(-50%);pointer-events:none"><polyline points="6 9 12 15 18 9"/></svg>
                        </div>
                    </div>
                    <div class="form-group">
                        <label class="form-label-figma">Threat Type <span class="required-figma">*</span></label>
                        <div style="position:relative">
                            <select class="form-input-figma form-select-figma" style="height:44px;appearance:none;padding-right:40px;width:100%;background:#fff">
                                <option>Regulatory / Compliance</option>
                                <option>Financial</option>
                                <option>Operational</option>
                                <option>Strategic</option>
                                <option>Market</option>
                                <option>Technology</option>
                                <option>Legal</option>
                                <option>Reputational</option>
                            </select>
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="position:absolute;right:12px;top:50%;transform:translateY(-50%);pointer-events:none"><polyline points="6 9 12 15 18 9"/></svg>
                        </div>
                    </div>
                </div>

                <div class="form-group" style="margin-bottom:20px">
                    <label class="form-label-figma">Risk Description <span class="required-figma">*</span></label>
                    <textarea class="form-input-figma" placeholder="Describe the risk in detail&hellip;" style="height:110px;min-height:110px;width:100%;background:#fff;resize:vertical"></textarea>
                </div>

                <div class="form-group" style="margin-bottom:20px;background:#fff;border-radius:12px;padding:20px 24px">
                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px">
                        <h4 style="font-size:16px;font-weight:700;color:#000;margin:0">Severity Score</h4>
                        <span id="ip-risk-severity-badge" style="display:inline-flex;align-items:center;padding:4px 14px;border-radius:20px;font-size:16px;font-weight:700;background:#eef0ff;color:#4f46e5">7.5/10</span>
                    </div>
                    <div style="padding:0 4px">
                        <input type="range" id="ip-risk-severity-slider" min="0" max="10" step="0.5" value="7.5" style="width:100%;height:6px;appearance:none;background:#d9d9d9;border-radius:12px;outline:none;cursor:pointer" />
                    </div>
                    <div style="display:flex;justify-content:space-between;font-size:13px;color:#4b5054;margin-top:6px">
                        <span>Low Impact</span>
                        <span>Medium</span>
                        <span>Critical</span>
                    </div>
                </div>

                <div class="form-group" style="margin-bottom:20px;background:#fff;border-radius:12px;padding:20px 24px">
                    <h4 style="font-size:16px;font-weight:700;color:#000;margin:0 0 12px 0">Initial Mitigation</h4>
                    <div id="ip-mitigation-steps">
                        <div class="ip-mitigation-step" style="display:flex;align-items:center;gap:10px;margin-bottom:10px">
                            <input type="text" class="form-input-figma" placeholder="Step 1: Immediate containment" style="height:44px;flex:1;background:#fff" />
                            <svg class="ip-remove-step" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="cursor:pointer;flex-shrink:0"><polyline points="3 6 5 6 21 6"/><path d="M19 6v14a2 2 0 0 1-2 2H7a2 2 0 0 1-2-2V6m3 0V4a2 2 0 0 1 2-2h4a2 2 0 0 1 2 2v2"/></svg>
                        </div>
                    </div>
                    <div id="ip-add-step-link" style="font-size:14px;color:#4f46e5;cursor:pointer;display:flex;align-items:center;gap:6px">
                        <svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                        + Add Step
                    </div>
                </div>

                <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:8px">
                    <div class="form-group">
                        <label class="form-label-figma">Responsible Party (Owner)</label>
                        <div style="position:relative">
                            <select class="form-input-figma form-select-figma" style="height:44px;appearance:none;padding-right:40px;width:100%;background:#fff">
                                <option>Assign Owner&hellip;</option>
                                <option>Fatima Al-Rashid</option>
                                <option>Omar Khayyam</option>
                                <option>Layla bint Hassan</option>
                                <option>Ahmad Hassan</option>
                            </select>
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="position:absolute;right:12px;top:50%;transform:translateY(-50%);pointer-events:none"><polyline points="6 9 12 15 18 9"/></svg>
                        </div>
                    </div>
                    <div class="form-group">
                        <label class="form-label-figma">Target Resolution Date</label>
                        <div style="position:relative">
                            <input type="text" class="form-input-figma" placeholder="dd/mm/yyyy" style="height:44px;width:100%;background:#fff" />
                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="position:absolute;right:12px;top:50%;transform:translateY(-50%);pointer-events:none"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
                        </div>
                    </div>
                </div>
            </div>
            <div class="modal-footer-figma" style="display:flex;justify-content:flex-end;align-items:center;gap:12px;padding:16px 32px;background:#fff;border-radius:0 0 16px 16px">
                <button class="btn-modal-figma btn-modal-cancel" @click="closeIpLogRiskModal()">Cancel</button>
                <button id="ip-add-risk-entry-btn" class="btn-modal-figma" style="display:flex;align-items:center;gap:8px;background:#e50303;color:#fff;border:none;border-radius:8px;padding:12px 24px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer">
                    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                    Add Risk Entry
                </button>
            </div>
        </div>
    </div>

    <div id="new-brief-modal" class="modal-overlay">
        <div class="modal-content">
            <div class="modal-header">
                <div class="modal-title">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" stroke="none">
                        <path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/>
                    </svg>
                    New Research Brief
                </div>
                <button class="modal-close" @click="closeNewBriefModal()">&times;</button>
            </div>
            <div class="modal-divider"></div>
            <div class="modal-body">
                <div class="form-row">
                    <div class="form-group">
                        <label class="form-label-figma">BRIEF TITLE <span class="required-figma">*</span></label>
                        <input type="text" class="form-input-figma" placeholder="e.g., islamic finTech Landscape 2025" style="height:40px" />
                    </div>
                    <div class="form-group">
                        <label class="form-label-figma">SECTOR/THEME <span class="required-figma">*</span></label>
                        <select class="form-input-figma form-select-figma" style="height:44px">
                            <option value="">Select Sector</option>
                            <option>FinTech</option>
                            <option>Sukuk & Capital Markets</option>
                            <option>Regulatory</option>
                            <option>Market Intelligence</option>
                            <option>Shari'ah Compliance</option>
                        </select>
                    </div>
                </div>
                <div class="form-group">
                    <label class="form-label-figma">OPPORTUNITY DESCRIPTION <span class="required-figma">*</span></label>
                    <textarea class="form-input-figma form-textarea-figma" placeholder="e.g., islamic finTech Landscape 2025" style="height:125px"></textarea>
                </div>
                <div class="form-row">
                    <div class="form-group">
                        <label class="form-label-figma">FINANCIAL VIABILITY SCORE</label>
                        <input type="text" class="form-input-figma" placeholder="0-200" style="height:40px" />
                    </div>
                    <div class="form-group">
                        <label class="form-label-figma">DATA SOURCES<span class="required-figma">*</span></label>
                        <input type="text" class="form-input-figma" placeholder="Bloomberg, Reuters, CBN" style="height:40px" />
                    </div>
                </div>
                <div class="form-group">
                    <label class="form-label-figma">SHARI'AH COMPLIANCE STATUS <span class="required-figma">*</span></label>
                    <select class="form-input-figma form-select-figma" style="height:44px">
                        <option>Compliant</option>
                        <option>Non-Compliant</option>
                        <option>Pending Review</option>
                    </select>
                </div>
                <div class="form-group" style="margin-top:8px">
                    <label class="form-label-figma">ATTACHMENTS (PDF/XLSX)</label>
                    <div class="form-upload-figma">
                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#667085" stroke-width="2">
                            <path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"></path>
                            <polyline points="17 8 12 3 7 8"></polyline>
                            <line x1="12" y1="3" x2="12" y2="15"></line>
                        </svg>
                        <span style="color:#000">Drag & Drop files or browse</span>
                    </div>
                </div>
            </div>
            <div class="modal-footer-figma">
                <button class="btn-modal-figma btn-modal-cancel" @click="closeNewBriefModal()">Cancel</button>
                <button class="btn-modal-figma btn-modal-draft" @click="closeNewBriefModal()">Save Draft</button>
                <button class="btn-modal-figma btn-modal-submit" @click="closeNewBriefModal()">
                    Submit Brief
                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
                        <path d="M5 12h14"></path>
                        <path d="m12 5 7 7-7 7"></path>
                    </svg>
                </button>
            </div>
        </div>


</div>
</template>
<script setup>
import { ref } from "vue";
const closeIpDetail = (...args) => { console.log('closeIpDetail called', args); };
const switchIpDetailTab = (...args) => { console.log('switchIpDetailTab called', args); };
const closeIpNewIdeaModal = (...args) => { console.log('closeIpNewIdeaModal called', args); };
const closeIpLogRiskModal = (...args) => { console.log('closeIpLogRiskModal called', args); };
const closeNewBriefModal = (...args) => { console.log('closeNewBriefModal called', args); };
</script>