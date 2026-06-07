<template>
<div>

            <div style="padding:24px">
                <div style="display:grid;grid-template-columns:repeat(4,1fr);gap:16px;margin-bottom:24px">
                    <div style="background:#fff;border-radius:12px;padding:20px;display:flex;flex-direction:column;gap:8px">
                        <div style="width:43px;height:43px;border-radius:12px;background:rgba(49,62,178,0.1);display:flex;align-items:center;justify-content:center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#313eb2" stroke-width="2"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg></div>
                        <div style="font-size:40px;font-weight:600;line-height:1;color:#313eb2">8</div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054">Affected Funds</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:20px;display:flex;flex-direction:column;gap:8px">
                        <div style="width:43px;height:43px;border-radius:12px;background:rgba(229,3,3,0.1);display:flex;align-items:center;justify-content:center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2"><path d="M10.29 3.86L1.82 18a2 2 0 0 0 1.71 3h16.94a2 2 0 0 0 1.71-3L13.71 3.86a2 2 0 0 0-3.42 0z"/><line x1="12" y1="9" x2="12" y2="13"/><line x1="12" y1="17" x2="12.01" y2="17"/></svg></div>
                        <div style="font-size:40px;font-weight:600;line-height:1;color:#e50303">8</div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054">High Impact Policies</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:20px;display:flex;flex-direction:column;gap:8px">
                        <div style="width:43px;height:43px;border-radius:12px;background:rgba(202,138,4,0.1);display:flex;align-items:center;justify-content:center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#ca8a04" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg></div>
                        <div style="font-size:40px;font-weight:600;line-height:1;color:#ca8a04">8</div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054">Under Review</div>
                    </div>
                    <div style="background:#fff;border-radius:12px;padding:20px;display:flex;flex-direction:column;gap:8px">
                        <div style="width:43px;height:43px;border-radius:12px;background:rgba(34,139,34,0.1);display:flex;align-items:center;justify-content:center"><svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg></div>
                        <div style="font-size:40px;font-weight:600;line-height:1;color:#228b22">61%</div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054">Analyzed this month</div>
                    </div>
                </div>
                <div style="background:#fff;border-radius:12px;padding:24px 16px">
                    <div style="display:flex;align-items:center;gap:12px;margin-bottom:24px">
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;width:368px"><input type="text" placeholder="Search" style="border:none;background:transparent;font-size:16px;color:#c4c4c4;outline:none;width:100%" /></div>
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:12px;background:#fff;font-size:16px;color:#000;cursor:pointer">All Themes<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg></div>
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:12px;background:#fff;font-size:16px;color:#000;cursor:pointer">All Impact Levels<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg></div>
                        <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer"><svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>Export</button>
                    </div>
                    <div style="border:1px solid #e5e5e5;border-radius:8px;overflow:hidden">
                        <div style="display:grid;grid-template-columns:200px 180px 100px 85px 95px 95px 65px 45px;gap:10px;padding:16px 24px;background:#e5e5e5;font-size:14px;font-weight:600;color:#000"><div>POLICY TITLE</div><div>SOURCE</div><div>THEME</div><div>DATE</div><div>IMPACT LEVEL</div><div>STATUS</div><div>AFFECTED FUNDS</div><div>ACTIONS</div></div>
                        <div style="display:grid;grid-template-columns:200px 180px 100px 85px 95px 95px 65px 45px;gap:10px;padding:16px 24px;border-bottom:1px solid #e5e5e5;align-items:center"><div style="font-size:14px;color:#0f151f">SEC Updates ESG Disclosure Requirements</div><div style="font-size:14px;color:#4b5054">Securities and Exchange Commission</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(49,62,178,0.1);color:#313eb2">ESG Compliance</span></div><div style="font-size:14px;color:#4b5054">Jan 15, 2024</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(34,139,34,0.1);color:#228b22">Low</span></div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:#e5e5e5;color:#4b5054">Implemented</span></div><div style="font-size:14px;color:#4b5054">12</div><div><span @click="showRwPolicyDetail()" style="color:#228b22;font-weight:600;font-size:14px;cursor:pointer">View</span></div></div>
                        <div style="display:grid;grid-template-columns:200px 180px 100px 85px 95px 95px 65px 45px;gap:10px;padding:16px 24px;border-bottom:1px solid #e5e5e5;align-items:center"><div style="font-size:14px;color:#0f151f">Central Bank Issues New Capital Requirements</div><div style="font-size:14px;color:#4b5054">Central Bank</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(34,139,34,0.1);color:#228b22">Capital</span></div><div style="font-size:14px;color:#4b5054">Jan 10, 2024</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(229,3,3,0.1);color:#e50303">High</span></div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(202,138,4,0.1);color:#ca8a04">Under Review</span></div><div style="font-size:14px;color:#4b5054">8</div><div><span @click="showRwPolicyDetail()" style="color:#228b22;font-weight:600;font-size:14px;cursor:pointer">View</span></div></div>
                        <div style="display:grid;grid-template-columns:200px 180px 100px 85px 95px 95px 65px 45px;gap:10px;padding:16px 24px;border-bottom:1px solid #e5e5e5;align-items:center"><div style="font-size:14px;color:#0f151f">ESG Taxonomy Framework Proposed</div><div style="font-size:14px;color:#4b5054">Ministry of Finance</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(49,62,178,0.1);color:#313eb2">ESG</span></div><div style="font-size:14px;color:#4b5054">Dec 28, 2023</div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(202,138,4,0.1);color:#ca8a04">Medium</span></div><div><span style="display:inline-block;padding:4px 12px;border-radius:11px;font-size:14px;background:rgba(34,139,34,0.1);color:#228b22">New</span></div><div style="font-size:14px;color:#4b5054">20</div><div><span @click="showRwPolicyDetail()" style="color:#228b22;font-weight:600;font-size:14px;cursor:pointer">View</span></div></div>
                    </div>
                    <div style="display:flex;align-items:center;justify-content:space-between;margin-top:24px;padding-top:24px;border-top:1px solid #e5e5e5">
                        <span style="font-size:14px;color:#000">Showing 1-5 of 47</span>
                        <div style="display:flex;gap:8px">
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">&lt;</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #228b22;border-radius:4px;background:#228b22;font-size:14px;font-weight:600;color:#fff;cursor:pointer">1</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">2</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">3</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">...</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">5</button>
                        </div>
                    </div>
                </div>
            </div>

            <div id="rw-add-data" class="ra-view" style="display:none;background:#f5f5f5;min-height:100%;padding:0">
                <div style="max-width:1360px;margin:0 auto;padding:0">

                    <div style="display:flex;align-items:center;justify-content:space-between;padding:20px 30px">
                        <div style="display:flex;align-items:center;gap:16px">
                            <div @click="showRwAddDataBack()" style="width:40px;height:40px;border-radius:8px;border:1px solid #e5e5e5;display:flex;align-items:center;justify-content:center;cursor:pointer;background:#fff">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                            </div>
                            <div>
                                <div style="font-size:28px;font-weight:700;color:#2d3643">Log New Policy Update</div>
                                <div style="font-size:15px;color:#4b5054;margin-top:4px">Document regulatory changes and analyze their impact on portfolio</div>
                            </div>
                        </div>
                        <div style="display:flex;align-items:center;gap:12px">
                            <button @click="showRwAddDataBack()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:15px;font-weight:600;color:#2d3643;cursor:pointer;font-family:inherit">
                                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                                Save Draft
                            </button>
                            <button @click="submitRwPolicyUpdate()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;background:#228b22;color:#fff;border:none;border-radius:8px;font-size:15px;font-weight:600;cursor:pointer;font-family:inherit">
                                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                                Submit Policy Update
                            </button>
                        </div>
                    </div>

                    <div style="display:grid;grid-template-columns:1fr 320px;gap:24px;padding:0 30px 30px">

                        <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:28px">

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="16"/><line x1="8" y1="12" x2="16" y2="12"/></svg>
                                Basic Info
                            </div>
                            <div style="height:1px;background:#e5e5e5;margin-bottom:20px"></div>

                            <div style="margin-bottom:20px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Policy Name*</label>
                                <input type="text" placeholder="SEC Updates..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none" />
                            </div>

                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:16px">
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Source*</label>
                                    <input type="text" placeholder="e.g., Securities and Exchange commission" style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none" />
                                </div>
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Date*</label>
                                    <div style="position:relative">
                                        <input type="text" value="02/02/2026" style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none" />
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="position:absolute;right:12px;top:50%;transform:translateY(-50%)"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
                                    </div>
                                </div>
                            </div>

                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:16px">
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Theme</label>
                                    <div style="display:flex;align-items:center;justify-content:space-between;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer;font-size:14px;color:#2d3643">
                                        <span>ESG Compliance</span>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                                    </div>
                                </div>
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Impact Level</label>
                                    <div style="display:flex;align-items:center;justify-content:space-between;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer;font-size:14px;color:#2d3643">
                                        <span>Medium Impact</span>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                                    </div>
                                </div>
                            </div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Change Description*</label>
                                <textarea rows="3" placeholder="Describe the regulatory..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
                                <div style="text-align:right;font-size:12px;color:#4b5054;margin-top:4px">0/500 Characters</div>
                            </div>

                            <div style="height:1px;background:#e5e5e5;margin:24px 0"></div>

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:8px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M12 20V10"/><path d="M18 20V4"/><path d="M6 20v-6"/></svg>
                                Affected Funds
                            </div>
                            <div style="font-size:13px;color:#4b5054;margin-bottom:14px">Select all funds that will be impacted by this policy change</div>

                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:8px;margin-bottom:12px">
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Tech Innovation VC Fund</span>
                                </div>
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Green Sukuk Fund</span>
                                </div>
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Global Infrastructure PE</span>
                                </div>
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Shari'ah Real Estate Trust</span>
                                </div>
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Microfinance Growth Fund</span>
                                </div>
                                <div style="display:flex;align-items:center;gap:10px;padding:10px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer">
                                    <input type="checkbox" style="width:16px;height:16px;accent-color:#228b22;cursor:pointer" />
                                    <span style="font-size:14px;color:#2d3643">Halal Biotech Index</span>
                                </div>
                            </div>
                            <div style="font-size:13px;color:#4b5054;font-weight:600">0 Funds Selected</div>

                            <div style="height:1px;background:#e5e5e5;margin:24px 0"></div>

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
                                Impact Analysis
                            </div>
                            <div style="height:1px;background:#e5e5e5;margin-bottom:20px"></div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Impact on Portfolio*</label>
                                <textarea rows="3" placeholder="Describe the regulatory..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
                                <div style="text-align:right;font-size:12px;color:#4b5054;margin-top:4px">0/500 Characters</div>
                            </div>

                            <div style="margin-bottom:16px">
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">Risk Score: <span id="rw-risk-score-val">5</span>/10 (<span id="rw-risk-label">Medium Risk</span>)</span>
                                </div>
                                <input id="rw-risk-slider" type="range" min="0" max="10" value="5" oninput="updateRwRisk(this.value)" style="width:100%;-webkit-appearance:none;height:6px;border-radius:3px;background:linear-gradient(to right, #eab308 0%, #eab308 50%, #d1d5db 50%, #d1d5db 100%);outline:none" />
                                <div style="display:flex;justify-content:space-between;font-size:12px;color:#4b5054;margin-top:4px">
                                    <span>Low Risk</span>
                                    <span>Medium Risk</span>
                                    <span>High Risk</span>
                                </div>
                            </div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Actionable Insight*</label>
                                <textarea rows="3" placeholder="Describe the regulatory..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
                            </div>

                            <div style="height:1px;background:#e5e5e5;margin:24px 0"></div>

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M21.21 15.89A10 10 0 1 1 8 2.83"/><path d="M22 12A10 10 0 0 0 12 2v10z"/></svg>
                                Supporting Documents
                            </div>
                            <div style="height:1px;background:#e5e5e5;margin-bottom:20px"></div>

                            <div style="border:2px dashed #228b22;border-radius:16px;padding:48px 24px;text-align:center;cursor:pointer">
                                <svg width="48" height="48" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="1.5" style="margin-bottom:12px"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                                <div style="font-size:16px;font-weight:600;color:#2d3643;margin-bottom:4px">Drag & drop files or browse</div>
                                <div style="font-size:13px;color:#4b5054">PDF, XLSX, DOCX, CSV · Max 25MB per file</div>
                            </div>

                            <div style="display:flex;align-items:center;justify-content:space-between;margin-top:28px;padding-top:20px;border-top:1px solid #e5e5e5">
                                <div>
                                    <button @click="showRwAddDataBack()" style="display:flex;align-items:center;gap:6px;padding:8px 16px;background:transparent;border:none;font-size:15px;color:#4b5054;cursor:pointer;font-family:inherit">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>
                                        Cancel
                                    </button>
                                </div>
                                <div style="display:flex;align-items:center;gap:12px">
                                    <button @click="showRwAddDataBack()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:15px;font-weight:600;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                                        Save Draft
                                    </button>
                                    <button @click="submitRwPolicyUpdate()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;background:#228b22;color:#fff;border:none;border-radius:8px;font-size:15px;font-weight:600;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                                        Submit Policy Update
                                    </button>
                                </div>
                            </div>
                        </div>

                        <div style="display:flex;flex-direction:column;gap:20px">

                            <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:22px">
                                <div style="font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">Submission Info</div>
                                <div style="display:flex;justify-content:space-between;padding:10px 0;border-bottom:1px solid #f0f0f0">
                                    <span style="font-size:14px;color:#4b5054">Status</span>
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">Draft</span>
                                </div>
                                <div style="display:flex;justify-content:space-between;padding:10px 0;border-bottom:1px solid #f0f0f0">
                                    <span style="font-size:14px;color:#4b5054">Created By</span>
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">Research Analyst</span>
                                </div>
                                <div style="display:flex;justify-content:space-between;padding:10px 0">
                                    <span style="font-size:14px;color:#4b5054">Last Modified</span>
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">Just now</span>
                                </div>
                            </div>

                            <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:22px">
                                <div style="font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">Shari'ah Compliance</div>
                                <div style="display:inline-flex;align-items:center;gap:8px;background:#dcfce7;padding:8px 16px;border-radius:8px;margin-bottom:12px">
                                    <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                                    <span style="font-size:14px;font-weight:600;color:#228b22">Compliant</span>
                                </div>
                                <div style="font-size:13px;color:#4b5054;line-height:1.5">This research brief meets Shari'ah compliance requirements based on sector and theme selection.</div>
                            </div>

                        </div>
                    </div>
                </div>
            </div>
        </div>

            <!-- Regulatory Policy Detail View -->
            <div id="rw-policy-detail" class="ra-view" style="display:none;background:#f4f0f0;min-height:100%;padding:0">
                <div style="max-width:1360px;margin:0 auto">

                    <!-- Top Nav -->
                    <div style="background:#fff;display:flex;align-items:center;justify-content:space-between;padding:12px 30px;border-bottom:1px solid #e5e5e5">
                        <div style="display:flex;align-items:center;gap:24px;flex:1">
                            <div @click="showRwPolicyDetailBack()" style="display:flex;align-items:center;gap:6px;cursor:pointer;color:#4b5054;font-size:14px;font-weight:600">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                                Back
                            </div>
                            <div style="display:flex;align-items:center;gap:8px;background:#f5f5f5;border:1px solid #a5a5a8;padding:7px 16px;border-radius:8px;flex:1;max-width:480px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>
                                <input type="text" placeholder="Search" style="border:none;background:transparent;font-size:15px;width:100%;outline:none;font-family:inherit" />
                            </div>
                        </div>
                        <div style="display:flex;align-items:center;gap:16px">
                            <div style="position:relative;cursor:pointer">
                                <svg width="22" height="22" viewBox="0 0 24 24" fill="none" stroke="#0f151f" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                                <span style="position:absolute;top:-4px;right:-6px;width:14px;height:14px;background:#e50303;border-radius:50%;display:flex;align-items:center;justify-content:center;font-size:9px;font-weight:600;color:#fff">3</span>
                            </div>
                            <div style="width:36px;height:36px;border-radius:50%;background:#d9d9d9;border:1px solid #bbb;cursor:pointer"></div>
                        </div>
                    </div>

                    <!-- Policy Header Card -->
                    <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);margin:24px 30px 20px;padding:28px 32px">
                        <div style="display:flex;align-items:flex-start;justify-content:space-between;margin-bottom:16px">
                            <div style="display:flex;align-items:flex-start;gap:14px;flex:1;min-width:0">
                                <div @click="showRwPolicyDetailBack()" style="cursor:pointer;flex-shrink:0;margin-top:4px">
                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                                </div>
                                <div>
                                    <h1 style="font-size:26px;font-weight:700;color:#2d3643;line-height:1.3;margin-bottom:12px">SEC Updates ESG Disclosure Requirements for Investment Funds</h1>
                                    <div style="display:flex;align-items:center;gap:10px;flex-wrap:wrap">
                                        <span style="display:inline-flex;align-items:center;padding:4px 14px;border-radius:20px;font-size:13px;font-weight:600;background:#fee2e2;color:#dc2626">High Impact</span>
                                        <span style="display:inline-flex;align-items:center;padding:4px 14px;border-radius:20px;font-size:13px;font-weight:600;background:#fef9c3;color:#b45309">Under Review</span>
                                        <span style="display:inline-flex;align-items:center;padding:4px 14px;border-radius:20px;font-size:13px;font-weight:600;background:#e8eaf6;color:#4f46e5">ESG Compliance</span>
                                    </div>
                                </div>
                            </div>
                            <button @click="alert('Exporting PDF...')" style="display:flex;align-items:center;gap:8px;padding:10px 18px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#4b5054;cursor:pointer;font-family:inherit;flex-shrink:0;margin-left:16px">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                Export PDF
                            </button>
                        </div>
                        <div style="display:flex;align-items:center;gap:28px;font-size:14px;color:#4b5054;flex-wrap:wrap">
                            <span style="display:flex;align-items:center;gap:6px">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18"/></svg>
                                <strong style="color:#2d3643">Affected Funds:</strong> 12 funds affected
                            </span>
                            <span style="display:flex;align-items:center;gap:6px">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
                                <strong style="color:#2d3643">Date:</strong> 1/12/2026
                            </span>
                            <span style="display:flex;align-items:center;gap:6px">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
                                <strong style="color:#2d3643">Source Organization:</strong> Securities and Exchange Commission
                            </span>
                        </div>
                    </div>

                    <!-- Tab Navigation -->
                    <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);margin:0 30px 20px;padding:0 4px;display:flex;gap:0;overflow-x:auto">
                        <div class="rw-detail-tab active" data-rw-detail-tab="overview" @click="switchRwDetailTab('overview')" style="padding:14px 24px;font-size:15px;font-weight:600;cursor:pointer;color:#228b22;border-bottom:3px solid #228b22;white-space:nowrap;flex-shrink:0">Overview</div>
                        <div class="rw-detail-tab" data-rw-detail-tab="impact" @click="switchRwDetailTab('impact')" style="padding:14px 24px;font-size:15px;font-weight:500;cursor:pointer;color:#4b5054;border-bottom:3px solid transparent;white-space:nowrap;flex-shrink:0">Impact Analysis</div>
                        <div class="rw-detail-tab" data-rw-detail-tab="documents" @click="switchRwDetailTab('documents')" style="padding:14px 24px;font-size:15px;font-weight:500;cursor:pointer;color:#4b5054;border-bottom:3px solid transparent;white-space:nowrap;flex-shrink:0">Documents &amp; Comments</div>
                    </div>

                    <!-- Main Content Grid -->
                    <div style="display:grid;grid-template-columns:1fr 340px;gap:20px;padding:0 30px 40px;align-items:start">

                        <!-- Left Column -->
                        <div style="display:flex;flex-direction:column;gap:20px;min-width:0">

                            <!-- Tab Panels -->
                            <div id="rw-detail-overview" class="rw-detail-panel active">

                                <!-- Card 1: Policy Overview -->
                                <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:28px 30px">
                                    <h2 style="font-size:18px;font-weight:700;color:#2d3643;margin-bottom:18px">Policy Overview</h2>
                                    <div style="height:1px;background:#e5e5e5;margin-bottom:18px"></div>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:16px">The Securities and Exchange Commission (SEC) has issued updated ESG disclosure requirements for investment funds, marking a significant shift in regulatory compliance standards. The new framework mandates comprehensive environmental, social, and governance reporting for all registered investment companies, requiring detailed disclosures on climate-related risks, diversity metrics, and governance structures.</p>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:16px">These regulations aim to enhance investor transparency and standardize ESG reporting across the investment industry. Fund managers must now disclose specific environmental impact metrics, including carbon footprint analysis, water usage, and waste management practices. Social metrics including workforce diversity, community engagement, and human rights policies must be reported annually.</p>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8">The governance component requires detailed reporting on board composition, executive compensation tied to ESG metrics, and shareholder engagement practices. Compliance deadlines are staggered, with larger funds required to comply within 12 months and smaller funds within 24 months of the effective date.</p>

                                    <h3 style="font-size:16px;font-weight:700;color:#2d3643;margin:24px 0 14px">Key Changes</h3>
                                    <div style="height:1px;background:#e5e5e5;margin-bottom:14px"></div>
                                    <ul style="font-size:15px;color:#4b5054;line-height:1.8;padding-left:20px;list-style-type:disc">
                                        <li style="margin-bottom:6px">Mandatory quarterly ESG reporting with standardized metrics framework</li>
                                        <li style="margin-bottom:6px">Third-party verification required for all environmental impact data</li>
                                        <li style="margin-bottom:6px">Climate-related disclosure requirements aligned with TCFD recommendations</li>
                                        <li style="margin-bottom:6px">Diversity and inclusion reporting including board composition targets</li>
                                        <li style="margin-bottom:6px">Enhanced governance transparency with shareholder voting record disclosures</li>
                                    </ul>
                                </div>

                                <!-- Card 2: Impact on Portfolio -->
                                <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:28px 30px">
                                    <h2 style="font-size:18px;font-weight:700;color:#2d3643;margin-bottom:18px">Impact on Portfolio</h2>
                                    <div style="height:1px;background:#e5e5e5;margin-bottom:18px"></div>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:16px">The new SEC ESG disclosure requirements will have significant implications across our fund portfolio. An estimated 12 funds within our current portfolio will be affected, representing approximately 35% of total assets under management. The primary impact areas include compliance costs, operational upgrades, and reporting infrastructure investments.</p>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:16px">Initial compliance cost projections range from $500,000 to $2 million per affected fund, depending on current ESG data collection capabilities and reporting infrastructure. Funds with existing ESG frameworks will face lower transition costs, while those without established processes will require more substantial investments in systems and personnel.</p>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8">However, these requirements also present opportunities for differentiation and investor attraction. Funds that demonstrate robust ESG compliance and transparency are likely to attract increased institutional investor interest, particularly from pension funds and sovereign wealth funds with mandated ESG investment criteria.</p>
                                </div>

                                <!-- Card 3: Actionable Insights -->
                                <div style="background:#f0fdf4;border:1px solid #86efac;border-radius:18px;padding:28px 30px">
                                    <h2 style="font-size:18px;font-weight:700;color:#166534;margin-bottom:14px">Actionable Insights</h2>
                                    <div style="height:1px;background:#86efac;margin-bottom:16px"></div>
                                    <ul style="font-size:15px;color:#166534;line-height:1.9;padding-left:20px;list-style-type:disc">
                                        <li style="margin-bottom:6px"><strong>Establish ESG compliance task force</strong> — Form a cross-functional team including legal, compliance, and investment operations to coordinate the implementation strategy</li>
                                        <li style="margin-bottom:6px"><strong>Conduct gap analysis</strong> — Evaluate current ESG data collection and reporting capabilities against new requirements to identify priority areas</li>
                                        <li style="margin-bottom:6px"><strong>Evaluate third-party ESG partners</strong> — Assess vendors for ESG data management, verification services, and reporting platform solutions</li>
                                        <li style="margin-bottom:6px"><strong>Develop phased rollout roadmap</strong> — Create a timeline for compliance, prioritizing high-impact funds and leveraging early adopter advantages</li>
                                        <li style="margin-bottom:6px"><strong>Allocate technology and training budget</strong> — Budget for ESG reporting software, data infrastructure, and staff training programs</li>
                                        <li style="margin-bottom:6px"><strong>Engage legal counsel</strong> — Work with regulatory specialists to ensure interpretation and implementation align with SEC expectations</li>
                                        <li style="margin-bottom:6px"><strong>Communicate updates to investors</strong> — Proactively inform investors about compliance progress and enhanced ESG transparency commitments</li>
                                    </ul>
                                </div>
                            </div>

                            <div id="rw-detail-impact" class="rw-detail-panel" style="display:none">
                                <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:28px 30px">
                                    <h2 style="font-size:18px;font-weight:700;color:#2d3643;margin-bottom:18px">Detailed Impact Analysis</h2>
                                    <div style="height:1px;background:#e5e5e5;margin-bottom:18px"></div>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:16px">The impact analysis examines the specific effects of the SEC ESG disclosure requirements on each affected fund within the portfolio. The analysis considers compliance costs, operational disruptions, competitive positioning, and potential investor sentiment shifts.</p>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.8;margin-bottom:20px">Quantitative analysis indicates an estimated total compliance cost of $8-12 million across the portfolio over the next 24 months, with ongoing annual compliance costs of $3-5 million thereafter. However, these costs are expected to be partially offset by increased investor inflows from ESG-mandated institutional investors.</p>
                                    <div style="border:1px solid #e5e5e5;border-radius:12px;overflow:hidden">
                                        <div style="display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:0;background:#e5e5e5;padding:12px 16px;font-size:13px;font-weight:600;color:#2d3643">
                                            <div>Fund Name</div><div style="text-align:center">Impact Level</div><div style="text-align:center">Est. Cost</div><div style="text-align:center">Priority</div>
                                        </div>
                                        <div style="display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:0;padding:12px 16px;border-bottom:1px solid #e5e5e5;font-size:14px;color:#4b5054">
                                            <div style="font-weight:600;color:#2d3643">Tech Innovation VC Fund</div>
                                            <div style="text-align:center"><span style="display:inline-flex;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fee2e2;color:#dc2626">High</span></div>
                                            <div style="text-align:center">$1.8M</div>
                                            <div style="text-align:center">1</div>
                                        </div>
                                        <div style="display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:0;padding:12px 16px;border-bottom:1px solid #e5e5e5;font-size:14px;color:#4b5054">
                                            <div style="font-weight:600;color:#2d3643">Green Sukuk Fund</div>
                                            <div style="text-align:center"><span style="display:inline-flex;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#fef9c3;color:#b45309">Medium</span></div>
                                            <div style="text-align:center">$1.2M</div>
                                            <div style="text-align:center">2</div>
                                        </div>
                                        <div style="display:grid;grid-template-columns:2fr 1fr 1fr 1fr;gap:0;padding:12px 16px;font-size:14px;color:#4b5054">
                                            <div style="font-weight:600;color:#2d3643">Global Infrastructure PE</div>
                                            <div style="text-align:center"><span style="display:inline-flex;padding:2px 10px;border-radius:10px;font-size:12px;font-weight:600;background:#dcfce7;color:#16a34a">Low</span></div>
                                            <div style="text-align:center">$0.6M</div>
                                            <div style="text-align:center">4</div>
                                        </div>
                                    </div>
                                </div>
                            </div>

                            <div id="rw-detail-documents" class="rw-detail-panel" style="display:none">
                                <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:28px 30px">
                                    <h2 style="font-size:18px;font-weight:700;color:#2d3643;margin-bottom:18px">Documents &amp; Comments</h2>
                                    <div style="height:1px;background:#e5e5e5;margin-bottom:18px"></div>
                                    <div style="display:flex;flex-direction:column;gap:12px;margin-bottom:24px">
                                        <div style="display:flex;align-items:center;gap:12px;padding:14px 16px;background:#f9fafb;border-radius:10px;cursor:pointer">
                                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                            <div style="flex:1"><div style="font-size:14px;font-weight:600;color:#2d3643">SEC_ESG_Disclosure_Rules_2026.pdf</div><div style="font-size:12px;color:#4b5054">3.2 MB &middot; Uploaded Jan 15, 2026</div></div>
                                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                        </div>
                                        <div style="display:flex;align-items:center;gap:12px;padding:14px 16px;background:#f9fafb;border-radius:10px;cursor:pointer">
                                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                            <div style="flex:1"><div style="font-size:14px;font-weight:600;color:#2d3643">Impact_Assessment_Report.xlsx</div><div style="font-size:12px;color:#4b5054">1.8 MB &middot; Uploaded Jan 18, 2026</div></div>
                                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                        </div>
                                        <div style="display:flex;align-items:center;gap:12px;padding:14px 16px;background:#f9fafb;border-radius:10px;cursor:pointer">
                                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                            <div style="flex:1"><div style="font-size:14px;font-weight:600;color:#2d3643">Compliance_Roadmap_v2.pptx</div><div style="font-size:12px;color:#4b5054">5.6 MB &middot; Uploaded Jan 22, 2026</div></div>
                                            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                        </div>
                                    </div>
                                    <div style="border:1px solid #e5e5e5;border-radius:12px;padding:18px 20px;margin-bottom:12px">
                                        <div style="display:flex;justify-content:space-between;margin-bottom:8px">
                                            <div><span style="font-size:14px;font-weight:600;color:#2d3643">Sarah James</span><span style="font-size:13px;color:#4b5054;margin-left:8px">Compliance Officer</span></div>
                                            <span style="font-size:13px;color:#4b5054">Jan 20, 2026</span>
                                        </div>
                                        <p style="font-size:14px;color:#4b5054;line-height:1.6">The new SEC requirements will significantly impact our reporting processes. I recommend we prioritize the gap analysis and begin vendor evaluation for ESG data management platforms immediately.</p>
                                    </div>
                                    <div style="border:1px solid #e5e5e5;border-radius:12px;padding:18px 20px;margin-bottom:12px">
                                        <div style="display:flex;justify-content:space-between;margin-bottom:8px">
                                            <div><span style="font-size:14px;font-weight:600;color:#2d3643">Dr. Amir Patel</span><span style="font-size:13px;color:#4b5054;margin-left:8px">Head of Investments</span></div>
                                            <span style="font-size:13px;color:#4b5054">Jan 22, 2026</span>
                                        </div>
                                        <p style="font-size:14px;color:#4b5054;line-height:1.6">Agreed. This also presents an opportunity to differentiate our ESG-compliant funds in the market. Let's coordinate with the marketing team on investor communication strategy.</p>
                                    </div>
                                    <div style="display:flex;gap:12px;margin-top:16px">
                                        <div style="width:36px;height:36px;border-radius:50%;background:#d9d9d9;flex-shrink:0"></div>
                                        <div style="flex:1;border:1px solid #e5e5e5;border-radius:10px;padding:12px 16px;font-size:14px;color:#c4c4c4">Add your comment or feedback...</div>
                                    </div>
                                </div>
                            </div>
                        </div>

                        <!-- Right Column Widgets -->
                        <div style="display:flex;flex-direction:column;gap:20px">

                            <!-- Widget 1: Quick Stats -->
                            <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:22px 24px">
                                <h3 style="font-size:16px;font-weight:700;color:#2d3643;margin-bottom:18px">Quick Stats</h3>
                                <div style="margin-bottom:18px">
                                    <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px">
                                        <span style="font-size:14px;color:#4b5054">Risk Score</span>
                                        <div style="display:flex;align-items:center;gap:6px">
                                            <span style="font-size:22px;font-weight:700;color:#dc2626">85</span>
                                            <span style="display:inline-flex;align-items:center;padding:2px 8px;border-radius:8px;font-size:11px;font-weight:600;background:#fee2e2;color:#dc2626">Critical</span>
                                        </div>
                                    </div>
                                    <div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden">
                                        <div style="height:100%;width:85%;background:#dc2626;border-radius:12px"></div>
                                    </div>
                                </div>
                                <div style="margin-bottom:18px">
                                    <div style="display:flex;justify-content:space-between;margin-bottom:6px">
                                        <span style="font-size:14px;color:#4b5054">Affected Funds</span>
                                        <span style="font-size:22px;font-weight:700;color:#228b22">12</span>
                                    </div>
                                    <div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden">
                                        <div style="height:100%;width:60%;background:#228b22;border-radius:12px"></div>
                                    </div>
                                </div>
                                <div style="border-top:1px solid #e5e5e5;padding-top:14px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px;color:#4b5054;margin-bottom:8px">
                                        <span>Submitted Date</span>
                                        <span style="font-weight:600;color:#2d3643">2024-02-01</span>
                                    </div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px;color:#4b5054">
                                        <span>Compliance Officer</span>
                                        <span style="font-weight:600;color:#2d3643">Sarah James</span>
                                    </div>
                                </div>
                            </div>

                            <!-- Widget 2: Actions -->
                            <div style="background:#fff;border-radius:18px;box-shadow:0 1px 4px rgba(0,0,0,0.05);padding:22px 24px">
                                <h3 style="font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">Actions</h3>
                                <div style="display:flex;flex-direction:column;gap:10px">
                                    <button @click="alert('Share with Team')" style="display:flex;align-items:center;gap:10px;width:100%;padding:12px 16px;border:1px solid #e5e5e5;border-radius:10px;background:#fff;font-size:14px;font-weight:500;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"/><polyline points="16 6 12 2 8 6"/><line x1="12" y1="2" x2="12" y2="15"/></svg>
                                        Share with Team
                                    </button>
                                    <button @click="alert('Added to Watch list')" style="display:flex;align-items:center;gap:10px;width:100%;padding:12px 16px;border:1px solid #e5e5e5;border-radius:10px;background:#fff;font-size:14px;font-weight:500;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"/></svg>
                                        Add to Watch list
                                    </button>
                                    <button @click="alert('Schedule Review')" style="display:flex;align-items:center;gap:10px;width:100%;padding:12px 16px;border:1px solid #e5e5e5;border-radius:10px;background:#fff;font-size:14px;font-weight:500;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><rect x="3" y="4" width="18" height="18" rx="2" ry="2"/><line x1="16" y1="2" x2="16" y2="6"/><line x1="8" y1="2" x2="8" y2="6"/><line x1="3" y1="10" x2="21" y2="10"/></svg>
                                        Schedule Review
                                    </button>
                                    <button @click="alert('Set Reminder')" style="display:flex;align-items:center;gap:10px;width:100%;padding:12px 16px;border:1px solid #e5e5e5;border-radius:10px;background:#fff;font-size:14px;font-weight:500;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
                                        Set Reminder
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>





</template>
<script setup>
import { ref } from "vue";
const showRwAddData = (...args) => { console.log('showRwAddData called', args); };
const showRwPolicyDetail = (...args) => { console.log('showRwPolicyDetail called', args); };
const showRwAddDataBack = (...args) => { console.log('showRwAddDataBack called', args); };
const submitRwPolicyUpdate = (...args) => { console.log('submitRwPolicyUpdate called', args); };
const showRwPolicyDetailBack = (...args) => { console.log('showRwPolicyDetailBack called', args); };
const alert = (...args) => { console.log('alert called', args); };
const switchRwDetailTab = (...args) => { console.log('switchRwDetailTab called', args); };
</script>