<template>
<div>
            <div id="ra-view-list" class="ra-view active">

                <div style="padding:30px;display:flex;justify-content:space-between;align-items:center">
                    <h2 style="font-size:20px;font-weight:700;color:#000">Risk Assessment</h2>
                    <button style="padding:8px 16px;background:#f5f5f5;border-radius:8px;font-size:14px;font-weight:600;color:#000;cursor:pointer;border:none">List View</button>
                </div>
                <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:20px;padding:0 30px;margin-bottom:30px">
                    <div style="background:#fff;border-radius:12px;padding:24px;display:flex;align-items:flex-start;position:relative;min-height:134px">
                        <div style="width:43px;height:43px;border-radius:12px;background:#313eb2;display:flex;align-items:center;justify-content:center;color:#fff;margin-right:auto"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg></div>
                        <div style="text-align:right;display:flex;flex-direction:column;align-items:flex-end;gap:8px"><div style="font-size:40px;font-weight:600;line-height:1;color:#313eb2">8</div></div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054;position:absolute;bottom:24px;left:24px">Total Risks</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:24px;display:flex;align-items:flex-start;position:relative;min-height:134px">
                        <div style="width:43px;height:43px;border-radius:12px;background:#e50303;display:flex;align-items:center;justify-content:center;color:#fff;margin-right:auto"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg></div>
                        <div style="text-align:right;display:flex;flex-direction:column;align-items:flex-end;gap:8px"><div style="font-size:40px;font-weight:600;line-height:1;color:#e50303">8</div></div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054;position:absolute;bottom:24px;left:24px">Critical Risks</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:24px;display:flex;align-items:flex-start;position:relative;min-height:134px">
                        <div style="width:43px;height:43px;border-radius:12px;background:#ca8a04;display:flex;align-items:center;justify-content:center;color:#fff;margin-right:auto"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg></div>
                        <div style="text-align:right;display:flex;flex-direction:column;align-items:flex-end;gap:8px"><div style="font-size:40px;font-weight:600;line-height:1;color:#ca8a04">8</div></div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054;position:absolute;bottom:24px;left:24px">Active Risks</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:24px;display:flex;align-items:flex-start;position:relative;min-height:134px">
                        <div style="width:43px;height:43px;border-radius:12px;background:#228b22;display:flex;align-items:center;justify-content:center;color:#fff;margin-right:auto"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg></div>
                        <div style="text-align:right;display:flex;flex-direction:column;align-items:flex-end;gap:8px"><div style="font-size:40px;font-weight:600;line-height:1;color:#228b22">61%</div></div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054;position:absolute;bottom:24px;left:24px">Avg. Mitigation</div>
                    </div>
                </div>
                <div style="background:#fff;border-radius:12px;margin:0 30px 30px;display:flex;flex-direction:column;overflow:hidden">
                    <div style="padding:20px 24px;display:flex;justify-content:space-between;border-bottom:1px solid #e5e5e5">
                        <input type="text" placeholder="Search" style="padding:10px 16px;border:1px solid #e5e5e5;border-radius:8px;width:400px;font-family:inherit;font-size:16px" />
                        <button style="display:flex;align-items:center;gap:8px;padding:10px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-family:inherit;font-size:16px;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3"/></svg>
                            Filter
                        </button>
                    </div>
                    <table style="width:100%;border-collapse:collapse;text-align:left">
                        <thead>
                            <tr>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">RISK ID</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">LINKED ITEM</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">THREAT TYPE</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">STATUS</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">SEVERITY</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">MITIGATION PROGRESS</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">OWNER</th>
                                <th style="padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#4b5054;text-transform:uppercase">ACTION</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="ra-row-click" @click="showRaDetail('RSK-001')">
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">RSK-001</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">Green Energy Fund Expansion</div><div style="font-size:12px;color:#4b5054">Investment Proposal</div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:6px 12px;border-radius:8px;font-size:14px;font-weight:600;background:#e5e5e5;color:#4b5054"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>Regulatory</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:6px;font-size:14px;font-weight:600;background:#dcfce7;color:#228b22">Active</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">85</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:12px"><div style="width:100px;height:8px;background:#d9d9d9;border-radius:4px;overflow:hidden"><div style="height:100%;width:60%;background:#228b22"></div></div><span style="font-size:12px;color:#4b5054;width:30px">60%</span></div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">Sarah James</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><a href="#" style="color:#228b22;font-weight:600;font-size:14px;text-decoration:none">View Details</a></td>
                            </tr>
                            <tr class="ra-row-click" @click="showRaDetail('RSK-002')">
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">RSK-002</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">Global Tech Solutions</div><div style="font-size:12px;color:#4b5054">International Growth</div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:6px 12px;border-radius:8px;font-size:14px;font-weight:600;background:#e5e5e5;color:#4b5054"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>Market</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:6px;font-size:14px;font-weight:600;background:#fef9c3;color:#ad751e">Under Review</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">72</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:12px"><div style="width:100px;height:8px;background:#d9d9d9;border-radius:4px;overflow:hidden"><div style="height:100%;width:45%;background:#ca8a04"></div></div><span style="font-size:12px;color:#4b5054;width:30px">45%</span></div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">Omar Khayyam</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><a href="#" style="color:#228b22;font-weight:600;font-size:14px;text-decoration:none">View Details</a></td>
                            </tr>
                            <tr class="ra-row-click" @click="showRaDetail('RSK-003')">
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">RSK-003</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">Solar Power Infrastructure</div><div style="font-size:12px;color:#4b5054">Infrastructure Fund</div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:6px 12px;border-radius:8px;font-size:14px;font-weight:600;background:#e5e5e5;color:#4b5054"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M12 2L2 7l10 5 10-5-10-5z"/><path d="M2 17l10 5 10-5"/><path d="M2 12l10 5 10-5"/></svg>Credit</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><span style="display:inline-flex;align-items:center;gap:6px;padding:4px 10px;border-radius:6px;font-size:14px;font-weight:600;background:#f3f4f6;color:#4b5054">Monitoring</span></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">50</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:12px"><div style="width:100px;height:8px;background:#d9d9d9;border-radius:4px;overflow:hidden"><div style="height:100%;width:80%;background:#313eb2"></div></div><span style="font-size:12px;color:#4b5054;width:30px">80%</span></div></td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5;font-size:14px;font-weight:600;color:#4b5054">Fatima Al-Rashid</td>
                                <td style="padding:16px 24px;border-bottom:1px solid #e5e5e5"><a href="#" style="color:#228b22;font-weight:600;font-size:14px;text-decoration:none">View Details</a></td>
                            </tr>
                        </tbody>
                    </table>
                    <div style="padding:20px 24px;display:flex;justify-content:space-between;align-items:center;border-top:1px solid #e5e5e5">
                        <span style="font-size:14px;color:#000">Showing 1-3 of 47</span>
                        <div style="display:flex;gap:8px">
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">&lt;</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #228b22;border-radius:4px;background:#228b22;font-size:14px;font-weight:600;color:#fff;cursor:pointer">1</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">2</button>
                            <span style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:none;font-size:14px;font-weight:600;color:#000">...</span>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">5</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">&gt;</button>
                        </div>
                    </div>
                </div>
            </div>

            <div id="ra-view-detail" class="ra-view" style="background:#f5f5f5;min-height:100%">
                <div style="padding:30px;max-width:1360px;margin:0 auto">
                    <div style="background:#fff;border-radius:16px;padding:24px 32px;margin-bottom:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                        <div style="display:flex;justify-content:space-between;align-items:flex-start">
                            <div style="display:flex;align-items:center;gap:16px">
                                <div id="ra-back-btn" @click="showRaList()" style="width:40px;height:40px;border-radius:8px;border:1px solid #e5e5e5;display:flex;align-items:center;justify-content:center;cursor:pointer">
                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                                </div>
                                <div>
                                    <h1 style="font-size:26px;font-weight:700;color:#000;margin:0">Green Energy Fund Expansion</h1>
                                    <div style="display:flex;align-items:center;gap:20px;margin-top:8px;font-size:14px;color:#4b5054;flex-wrap:wrap">
                                        <span><strong style="color:#000">Risk ID:</strong> RSK-001</span>
                                        <span><strong style="color:#000">Date:</strong> 1/12/2026</span>
                                        <span><strong style="color:#000">Proposal Type:</strong> Investment Proposal</span>
                                    </div>
                                </div>
                            </div>
                            <div style="display:flex;align-items:center;gap:12px">
                                <span style="display:inline-flex;align-items:center;padding:4px 14px;border-radius:20px;font-size:14px;font-weight:600;background:#dcfce7;color:#228b22">Active</span>
                                <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                                    Export PDF
                                </button>
                            </div>
                        </div>
                    </div>

                    <div style="background:#fff;border-radius:16px 16px 0 0;padding:0 32px;display:flex;border-bottom:1px solid #e5e5e5;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                        <button class="ra-tab-btn active" data-ra-detail-tab="overview" @click="switchRaDetailTab('overview')">Overview</button>
                        <button class="ra-tab-btn" data-ra-detail-tab="mitigation" @click="switchRaDetailTab('mitigation')">Mitigation Plan</button>
                        <button class="ra-tab-btn" data-ra-detail-tab="timeline" @click="switchRaDetailTab('timeline')">Timeline & History</button>
                    </div>

                    <div style="display:grid;grid-template-columns:1fr 340px;gap:24px;margin-top:24px">
                        <div>
                            <div id="ra-detail-overview" class="ra-detail-panel active">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 12px 0">Risk Description</h3>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.7;margin:0">The expansion of the Green Energy Fund into new emerging markets introduces significant ESG disclosure requirements and regulatory compliance burdens. Current regulatory frameworks across target jurisdictions (Southeast Asia, MENA) lack harmonization, creating operational complexity in reporting obligations. The fund must navigate differing Shari'ah governance standards, environmental impact disclosure mandates, and cross-border data privacy regulations. Failure to adequately address these compliance requirements could result in regulatory sanctions, reputational damage, and restricted market access. Additionally, the evolving nature of ESG regulations in these regions requires continuous monitoring and adaptation of reporting frameworks, potentially increasing operational overhead and compliance costs by an estimated 15-20% over the next fiscal year.</p>
                                </div>
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 12px 0">Impact Assessment</h3>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.7;margin:0">The compliance burden associated with multi-jurisdictional ESG reporting is projected to increase operational overhead by 15-20% annually. Restructuring costs for alignment with diverse regulatory standards could reach USD 2-3M, impacting the fund's cost structure and investor returns. The operational overhead of managing multiple reporting frameworks may divert resources from core investment activities. Investor attractiveness could be affected if transparency and compliance standards are not consistently maintained across all markets. ESG alignment with global standards (GRI, SASB, AAOIFI) will require significant enhancements to existing reporting infrastructure, including investment in data management systems and specialized compliance personnel.</p>
                                </div>
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Affected Investments</h3>
                                    <div style="display:flex;flex-direction:column;gap:12px">
                                        <div style="display:flex;align-items:center;justify-content:space-between;border:1px solid #e5e5e5;border-radius:12px;padding:16px 20px">
                                            <div style="display:flex;align-items:center;gap:12px">
                                                <div style="width:40px;height:40px;border-radius:10px;background:#dcfce7;display:flex;align-items:center;justify-content:center">
                                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"/></svg>
                                                </div>
                                                <div><div style="font-size:15px;font-weight:600;color:#000">Solar Power Infrastructure Fund</div><div style="font-size:13px;color:#4b5054">Portfolio Value: $12.5M</div></div>
                                            </div>
                                            <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:20px;font-size:13px;font-weight:600;background:#fee2e2;color:#dc2626">High Exposure</span>
                                        </div>
                                        <div style="display:flex;align-items:center;justify-content:space-between;border:1px solid #e5e5e5;border-radius:12px;padding:16px 20px">
                                            <div style="display:flex;align-items:center;gap:12px">
                                                <div style="width:40px;height:40px;border-radius:10px;background:#dcfce7;display:flex;align-items:center;justify-content:center">
                                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"/></svg>
                                                </div>
                                                <div><div style="font-size:15px;font-weight:600;color:#000">Islamic Microfinance Sukuk</div><div style="font-size:13px;color:#4b5054">Portfolio Value: $8.2M</div></div>
                                            </div>
                                            <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:20px;font-size:13px;font-weight:600;background:#fef9c3;color:#ca8a04">Medium Exposure</span>
                                        </div>
                                        <div style="display:flex;align-items:center;justify-content:space-between;border:1px solid #e5e5e5;border-radius:12px;padding:16px 20px">
                                            <div style="display:flex;align-items:center;gap:12px">
                                                <div style="width:40px;height:40px;border-radius:10px;background:#dcfce7;display:flex;align-items:center;justify-content:center">
                                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><rect x="2" y="7" width="20" height="14" rx="2"/><path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"/></svg>
                                                </div>
                                                <div><div style="font-size:15px;font-weight:600;color:#000">Halal Supply Chain REIT</div><div style="font-size:13px;color:#4b5054">Portfolio Value: $6.7M</div></div>
                                            </div>
                                            <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:20px;font-size:13px;font-weight:600;background:#fef9c3;color:#ca8a04">Medium Exposure</span>
                                        </div>
                                    </div>
                                </div>
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 12px 0">Comments & Feedback</h3>
                                    <div style="background:#f9fafb;border-radius:12px;padding:16px 20px">
                                        <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
                                            <div>
                                                <div style="font-size:15px;font-weight:600;color:#000">Dr. Hassan Adamu</div>
                                                <div style="font-size:13px;color:#4b5054">Senior Supervisor</div>
                                            </div>
                                            <div style="font-size:13px;color:#4b5054">2024-04-16</div>
                                        </div>
                                        <p style="font-size:14px;color:#4b5054;line-height:1.6;margin:0">The ESG compliance risks outlined require immediate attention. I recommend engaging with local regulatory consultants in each target market to ensure full alignment with disclosure requirements. The Shari'ah governance divergence between jurisdictions is particularly concerning and should be addressed as a priority item in the mitigation plan.</p>
                                    </div>
                                </div>
                            </div>
                            <div id="ra-detail-mitigation" class="ra-detail-panel">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Mitigation Plan</h3>
                                    <div style="display:flex;flex-direction:column;gap:16px">
                                        <div style="display:flex;align-items:flex-start;gap:14px;padding:16px;background:#f9fafb;border-radius:10px">
                                            <div style="width:28px;height:28px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;color:#fff;font-size:12px;flex-shrink:0">&#10003;</div>
                                            <div><div style="font-size:15px;font-weight:600;color:#000">Engage Regulatory Consultants</div><div style="font-size:13px;color:#4b5054;margin-top:2px">Hire local ESG compliance consultants in each target jurisdiction to map regulatory requirements and identify gaps. Target completion: Q2 2026.</div><div style="font-size:12px;color:#228b22;margin-top:4px">Completed · Mar 15, 2026</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:14px;padding:16px;background:#f9fafb;border-radius:10px">
                                            <div style="width:28px;height:28px;border-radius:50%;background:#fef9c3;border:2px solid #ca8a04;display:flex;align-items:center;justify-content:center;color:#ca8a04;font-size:12px;font-weight:700;flex-shrink:0">2</div>
                                            <div><div style="font-size:15px;font-weight:600;color:#000">Standardize Reporting Framework</div><div style="font-size:13px;color:#4b5054;margin-top:2px">Develop a unified ESG reporting framework aligned with GRI, SASB, and AAOIFI standards. Implement centralized data collection system.</div><div style="font-size:12px;color:#ca8a04;margin-top:4px">In Progress · Due Jun 30, 2026</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:14px;padding:16px;background:#f9fafb;border-radius:10px">
                                            <div style="width:28px;height:28px;border-radius:50%;background:#e5e5e5;display:flex;align-items:center;justify-content:center;color:#999;font-size:12px;flex-shrink:0">3</div>
                                            <div><div style="font-size:15px;font-weight:600;color:#999">Compliance Training Program</div><div style="font-size:13px;color:#999;margin-top:2px">Develop and deliver compliance training for investment teams across all target markets. Cover ESG disclosure requirements and Shari'ah governance standards.</div></div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                            <div id="ra-detail-timeline" class="ra-detail-panel">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Activity Timeline</h3>
                                    <div style="display:flex;flex-direction:column;gap:16px">
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#fff;font-size:10px">&#10003;</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#000">Risk Identified</div><div style="font-size:12px;color:#4b5054">Sarah James · Dec 15, 2025</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#fff;font-size:10px">&#10003;</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#000">Risk Assessment Completed</div><div style="font-size:12px;color:#4b5054">Review Committee · Jan 10, 2026</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#fff;font-size:10px">&#10003;</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#000">Initial Mitigation Implemented</div><div style="font-size:12px;color:#4b5054">Sarah James · Mar 15, 2026</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#fef9c3;border:2px solid #ca8a04;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#ca8a04;font-size:10px;font-weight:700">4</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#000">Standardization Framework (Current)</div><div style="font-size:12px;color:#4b5054">Started Apr 1, 2026 · Due Jun 30, 2026</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#e5e5e5;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#999;font-size:10px">5</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#999">Compliance Training</div><div style="font-size:12px;color:#999">Pending framework completion</div></div>
                                        </div>
                                        <div style="display:flex;align-items:flex-start;gap:12px">
                                            <div style="width:24px;height:24px;border-radius:50%;background:#e5e5e5;display:flex;align-items:center;justify-content:center;flex-shrink:0;color:#999;font-size:10px">6</div>
                                            <div><div style="font-size:14px;font-weight:600;color:#999">Risk Review & Closure</div><div style="font-size:12px;color:#999">Pending all mitigation steps</div></div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <div>
                            <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Key Metrics</h3>
                                <div style="margin-bottom:16px">
                                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px">
                                        <span style="font-size:14px;font-weight:600;color:#000">Severity Level</span>
                                        <span style="display:inline-flex;align-items:center;padding:2px 10px;border-radius:12px;font-size:13px;font-weight:600;background:#fee2e2;color:#dc2626">Critical</span>
                                    </div>
                                    <div style="display:flex;align-items:center;gap:12px">
                                        <span style="font-size:28px;font-weight:700;color:#000">85</span>
                                        <div style="flex:1;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:85%;background:#e50303;border-radius:12px"></div></div>
                                    </div>
                                </div>
                                <div>
                                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px">
                                        <span style="font-size:14px;font-weight:600;color:#000">Mitigation Progress</span>
                                        <span style="font-size:14px;font-weight:600;color:#228b22">60%</span>
                                    </div>
                                    <div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:60%;background:#228b22;border-radius:12px"></div></div>
                                </div>
                                <div style="margin-top:16px;padding-top:16px;border-top:1px solid #e5e5e5">
                                    <div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:8px"><span style="color:#4b5054">Submitted Date</span><span style="font-weight:600;color:#000">2024-02-01</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:8px"><span style="color:#4b5054">Threat Resolution</span><span style="display:inline-flex;align-items:center;padding:2px 8px;border-radius:8px;font-size:12px;font-weight:600;background:#e5e5e5;color:#4b5054">Regulatory</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">Risk Owner</span><span style="font-weight:600;color:#000">Sarah James</span></div>
                                </div>
                            </div>

                            <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Actions</h3>
                                <div style="display:flex;flex-direction:column;gap:10px">
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
                                        Update Progress
                                    </button>
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#313eb2;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                                        Mark as Resolved
                                    </button>
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#fff;color:#000;border:1px solid #e5e5e5;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>
                                        Edit Risk Details
                                    </button>
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#fff;color:#000;border:1px solid #e5e5e5;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                        Export Report
                                    </button>
                                </div>
                            </div>

                            <div style="background:#fff;border-radius:16px;padding:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Severity Heatmap</h3>
                                <div style="display:flex;height:32px;border-radius:16px;overflow:hidden;margin-bottom:8px">
                                    <div style="flex:1;background:#228b22"></div>
                                    <div style="flex:1;background:#eab308"></div>
                                    <div style="flex:1;background:#f97316"></div>
                                    <div style="flex:1;background:#e50303"></div>
                                </div>
                                <div style="display:flex;justify-content:space-between;font-size:12px;color:#4b5054">
                                    <span>Low</span>
                                    <span>Medium</span>
                                    <span>High</span>
                                    <span>Critical</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>


</div>
</template>
<script setup>
import { ref } from "vue";
const showRaDetail = (...args) => { console.log('showRaDetail called', args); };
const showRaList = (...args) => { console.log('showRaList called', args); };
const switchRaDetailTab = (...args) => { console.log('switchRaDetailTab called', args); };
</script>