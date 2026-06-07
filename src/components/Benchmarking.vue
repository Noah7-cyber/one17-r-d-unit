<template>
<div>

            <div style="padding:0 24px 24px">
                <div style="display:grid;grid-template-columns:repeat(5,1fr);gap:16px;margin-top:24px;margin-bottom:24px">
                    <div style="background:#fff;border-radius:12px;padding:16px 20px;height:110px;display:flex;flex-direction:column;justify-content:space-between"><div style="font-size:40px;font-weight:600;color:#313eb2;line-height:1.2">8</div><div style="font-size:16px;font-weight:400;color:#4b5054">Peer Funds Tracked</div></div>
                    <div style="background:#fff;border-radius:12px;padding:16px 20px;height:110px;display:flex;flex-direction:column;justify-content:space-between"><div style="font-size:40px;font-weight:600;color:#313eb2;line-height:1.2">8%</div><div style="font-size:16px;font-weight:400;color:#4b5054">Avg. 1Y Return</div></div>
                    <div style="background:#fff;border-radius:12px;padding:16px 20px;height:110px;display:flex;flex-direction:column;justify-content:space-between"><div style="font-size:40px;font-weight:600;color:#313eb2;line-height:1.2">65</div><div style="font-size:16px;font-weight:400;color:#4b5054">Avg. Governance Score</div></div>
                    <div style="background:#fff;border-radius:12px;padding:16px 20px;height:110px;display:flex;flex-direction:column;justify-content:space-between"><div style="font-size:40px;font-weight:600;color:#313eb2;line-height:1.2">82</div><div style="font-size:16px;font-weight:400;color:#4b5054">Avg. ESG Score</div></div>
                    <div style="background:#fff;border-radius:12px;padding:16px 20px;height:110px;display:flex;flex-direction:column;justify-content:space-between"><div style="font-size:40px;font-weight:600;color:#313eb2;line-height:1.2">85</div><div style="font-size:16px;font-weight:400;color:#4b5054">Shari'ah Compliant</div></div>
                </div>
                <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px;background:#fff;border-radius:12px;padding:16px 24px">
                    <div style="display:flex;align-items:center;gap:12px">
                        <div style="display:flex;align-items:center;gap:8px;padding:10px 16px;border:1px solid #e5e5e5;border-radius:12px;font-size:16px;color:#000;cursor:pointer;background:#fff">All Fund Types<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="color:#4b5054"><polyline points="6 9 12 15 18 9"/></svg></div>
                        <div style="display:flex;align-items:center;gap:8px;padding:10px 16px;border:1px solid #e5e5e5;border-radius:12px;font-size:16px;color:#000;cursor:pointer;background:#fff">All Compliance<svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="color:#4b5054"><polyline points="6 9 12 15 18 9"/></svg></div>
                    </div>
                    <div style="display:flex;align-items:center;gap:12px">
                        <div style="display:flex;align-items:center;background:rgba(229,229,229,0.6);border-radius:12px;padding:3px">
                            <button id="bm-cards-btn" style="display:flex;align-items:center;gap:8px;padding:8px 16px;border-radius:8px;border:none;background:#fff;font-size:14px;font-weight:600;color:#228b22;cursor:pointer"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>Cards</button>
                            <button id="bm-matrix-btn" style="display:flex;align-items:center;gap:8px;padding:8px 16px;border-radius:8px;border:none;background:transparent;font-size:14px;font-weight:600;color:#000;cursor:pointer"><svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>Matrix</button>
                        </div>
                        <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer"><svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>Export</button>
                    </div>
                </div>
                <div id="bm-matrix-view" style="display:none">
                    <div style="background:#fff;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:16px">
                            <div style="display:flex;align-items:center;gap:8px;padding:10px 16px;border:1px solid #e5e5e5;border-radius:8px;width:712px;font-size:16px;color:#c4c4c4"><svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>Search</div>
                            <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:16px;color:#000;cursor:pointer"><svg width="16" height="16" viewBox="0 0 24 24" fill="currentColor" stroke="none"><polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3"/></svg>Filter</button>
                        </div>
                        <table style="width:100%;border-collapse:collapse">
                            <thead><tr>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">Fund Name</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">Fund Type</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">1Y Return</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">3Y Return</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">5Y Return</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">AUM ($M)</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">Alignment</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">Compliance</th>
                                <th style="text-align:left;padding:12px;font-size:14px;font-weight:600;color:#4b5054;background:#e5e5e5">Updated</th>
                            </tr></thead>
                            <tbody>
                                <tr class="bm-matrix-row"><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5;font-weight:600">Tech Innovation VC Fund</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:8px;font-size:12px;font-weight:500;background:#dcfce7;color:#228b22">Venture Capital</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">22.1%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">42.1%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">122.1%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">280</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><div style="width:68px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:92%;background:#228b22;border-radius:12px"></div></div></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="padding:4px 10px;border-radius:6px;font-size:12px;font-weight:500;background:#dcfce7;color:#228b22">Compliant</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">2h ago</td></tr>
                                <tr class="bm-matrix-row"><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5;font-weight:600">Green Sukuk Fund</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:8px;font-size:12px;font-weight:500;background:#eff6ff;color:#313eb2">Sukuk</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">8.5%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">24.3%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">45.8%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">420</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><div style="width:68px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:78%;background:#228b22;border-radius:12px"></div></div></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="padding:4px 10px;border-radius:6px;font-size:12px;font-weight:500;background:#dcfce7;color:#228b22">Compliant</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">5h ago</td></tr>
                                <tr class="bm-matrix-row"><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5;font-weight:600">Global Infrastructure PE</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:8px;font-size:12px;font-weight:500;background:#fef9c3;color:#946325">Private Equity</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">15.3%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">38.7%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">95.2%</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">1,200</td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><div style="width:68px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:85%;background:#228b22;border-radius:12px"></div></div></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5"><span style="padding:4px 10px;border-radius:6px;font-size:12px;font-weight:500;background:#fef9c3;color:#946325">Review</span></td><td style="padding:16px 12px;font-size:14px;color:#2d3643;border-bottom:1px solid #e5e5e5">1d ago</td></tr>
                            </tbody>
                        </table>
                        <div style="display:flex;align-items:center;justify-content:space-between;margin-top:16px;padding-top:16px;border-top:1px solid #e5e5e5">
                            <span style="font-size:14px;color:#2d3643">Showing 1-3 of 47</span>
                            <div style="display:flex;align-items:center;gap:8px">
                                <button disabled style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643;opacity:0.5">&lt;</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #228b22;background:#228b22;color:#fff">1</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643">2</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643">3</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643">...</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643">5</button>
                                <button style="width:32px;height:32px;border-radius:4px;display:flex;align-items:center;justify-content:center;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#2d3643">&gt;</button>
                            </div>
                        </div>
                    </div>
                </div>
                <div id="bm-cards-view">
                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Tech Innovation VC Fund</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Venture Capital</span>
                                    <span style="font-size:13px;color:#4b5054">$280M AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">22.1%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">42.1%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">122.1%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">82</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">65</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>

                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Green Sukuk Fund</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Sukuk / Fixed Income</span>
                                    <span style="font-size:13px;color:#4b5054">$420M AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">8.5%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">24.3%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">45.8%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">78</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">72</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>

                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Global Infrastructure PE</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Private Equity</span>
                                    <span style="font-size:13px;color:#4b5054">$1.2B AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">15.3%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">38.7%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">95.2%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">88</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">81</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>

                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Shari'ah Real Estate Trust</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">REIT</span>
                                    <span style="font-size:13px;color:#4b5054">$680M AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">11.2%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">28.6%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">58.4%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">71</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">68</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>

                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Microfinance Growth Fund</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Microfinance</span>
                                    <span style="font-size:13px;color:#4b5054">$180M AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">18.9%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">52.3%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">148.7%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">64</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">59</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>

                        <div class="bm-fund-card" style="background:#fff;border-radius:18px;padding:24px;box-shadow:0 1px 4px rgba(0,0,0,0.05);display:flex;flex-direction:column;gap:0">
                            <div style="margin-bottom:16px">
                                <div style="font-size:20px;font-weight:700;color:#000">Halal Biotech Index</div>
                                <div style="display:flex;align-items:center;justify-content:space-between;margin-top:6px">
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:20px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Sector Equity</span>
                                    <span style="font-size:13px;color:#4b5054">$950M AUM</span>
                                </div>
                            </div>
                            <div style="border-top:1px solid #f0f0f0;padding:14px 0">
                                <div style="display:flex;flex-direction:column;gap:8px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">1Y Return</span><span style="font-weight:700;color:#228b22">25.4%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">3Y Return</span><span style="font-weight:700;color:#228b22">61.8%</span></div>
                                    <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">5Y Return</span><span style="font-weight:700;color:#228b22">186.3%</span></div>
                                </div>
                            </div>
                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:12px;margin-bottom:16px">
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">Governance</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">90</div>
                                </div>
                                <div style="background:#f9fafb;border-radius:10px;padding:12px;text-align:center">
                                    <div style="font-size:12px;color:#4b5054;margin-bottom:2px">ESG Score</div>
                                    <div style="font-size:22px;font-weight:700;color:#000">85</div>
                                </div>
                            </div>
                            <button class="bm-view-analysis" style="width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:15px;font-weight:600;cursor:pointer" @click="showBmDetail()">View Full Analysis</button>
                        </div>
                    </div>
                </div>
            </div>

            <div id="bm-view-detail" class="ra-view" style="background:#f5f5f5;min-height:100%">
                <div style="padding:30px;max-width:1360px;margin:0 auto">
                    <div style="background:#fff;border-radius:16px;padding:24px 32px;margin-bottom:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                        <div style="display:flex;justify-content:space-between;align-items:flex-start">
                            <div style="display:flex;align-items:center;gap:16px">
                                <div id="bm-back-btn" @click="showBmList()" style="width:40px;height:40px;border-radius:8px;border:1px solid #e5e5e5;display:flex;align-items:center;justify-content:center;cursor:pointer">
                                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                                </div>
                                <div>
                                    <div style="display:flex;align-items:center;gap:12px">
                                        <h1 style="font-size:24px;font-weight:700;color:#000;margin:0">Al-Baraka Islamic Growth Fund</h1>
                                        <span style="display:inline-flex;align-items:center;padding:4px 12px;border-radius:20px;font-size:13px;font-weight:600;background:#dcfce7;color:#228b22">Shari'ah Compliant</span>
                                    </div>
                                    <div style="display:flex;align-items:center;gap:24px;margin-top:8px;font-size:14px;color:#4b5054;flex-wrap:wrap">
                                        <span><strong style="color:#000">Fund Category:</strong> Ethical Fund</span>
                                        <span><strong style="color:#000">Date:</strong> 1/12/2026</span>
                                        <span><strong style="color:#000">AUM:</strong> $450M AUM</span>
                                    </div>
                                </div>
                            </div>
                            <div style="display:flex;align-items:center;gap:12px">
                                <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                                    Export PDF
                                </button>
                                <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;background:#228b22;color:#fff;border:none;border-radius:8px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                    <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>
                                    Edit Data
                                </button>
                            </div>
                        </div>
                    </div>

                    <div style="background:#fff;border-radius:16px 16px 0 0;padding:0 32px;display:flex;border-bottom:1px solid #e5e5e5;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                        <button class="bm-tab-btn active" data-bm-detail-tab="overview" @click="switchBmDetailTab('overview')">Overview</button>
                        <button class="bm-tab-btn" data-bm-detail-tab="performance" @click="switchBmDetailTab('performance')">Performance Analysis</button>
                        <button class="bm-tab-btn" data-bm-detail-tab="competitive" @click="switchBmDetailTab('competitive')">Competitive Analysis</button>
                    </div>

                    <div style="display:grid;grid-template-columns:1fr 340px;gap:24px;margin-top:24px">
                        <div>
                            <div id="bm-detail-overview" class="bm-detail-panel active">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 20px 0">Key Performance Metrics</h3>
                                    <div style="display:grid;grid-template-columns:repeat(3,1fr);gap:24px">
                                        <div style="text-align:center;padding:16px;background:#f9fafb;border-radius:12px">
                                            <div style="font-size:36px;font-weight:700;color:#228b22;line-height:1.1">12.5%</div>
                                            <div style="font-size:14px;color:#4b5054;margin-top:4px">1-Year Return</div>
                                            <div style="font-size:12px;color:#228b22;margin-top:2px">+1.5% vs Avg</div>
                                        </div>
                                        <div style="text-align:center;padding:16px;background:#f9fafb;border-radius:12px">
                                            <div style="font-size:36px;font-weight:700;color:#228b22;line-height:1.1">32.5%</div>
                                            <div style="font-size:14px;color:#4b5054;margin-top:4px">3-Year Return</div>
                                            <div style="font-size:12px;color:#228b22;margin-top:2px">+1.5% vs Avg</div>
                                        </div>
                                        <div style="text-align:center;padding:16px;background:#f9fafb;border-radius:12px">
                                            <div style="font-size:36px;font-weight:700;color:#228b22;line-height:1.1">62.5%</div>
                                            <div style="font-size:14px;color:#4b5054;margin-top:4px">5-Year Return</div>
                                            <div style="font-size:12px;color:#228b22;margin-top:2px">+1.5% vs Avg</div>
                                        </div>
                                    </div>
                                </div>

                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 20px 0">Multi-Metric Comparison</h3>
                                    <div style="display:flex;justify-content:center;padding:10px 0">
                                        <svg viewBox="0 0 300 300" width="300" height="300">
                                            <polygon points="150,30 260,90 260,210 150,270 40,210 40,90" fill="none" stroke="#d9d9d9" stroke-width="1"/>
                                            <polygon points="150,50 240,100 240,200 150,250 60,200 60,100" fill="none" stroke="#d9d9d9" stroke-width="1"/>
                                            <polygon points="150,70 220,110 220,190 150,230 80,190 80,110" fill="none" stroke="#d9d9d9" stroke-width="1"/>
                                            <polygon points="150,90 200,120 200,180 150,210 100,180 100,120" fill="none" stroke="#d9d9d9" stroke-width="1"/>
                                            <polygon points="150,110 180,130 180,170 150,190 120,170 120,130" fill="none" stroke="#d9d9d9" stroke-width="1"/>
                                            <polygon points="150,60 230,100 230,200 150,240 70,200 70,100" fill="#228b22" fill-opacity="0.15" stroke="#228b22" stroke-width="2"/>
                                            <circle cx="150" cy="60" r="3" fill="#228b22"/>
                                            <circle cx="230" cy="100" r="3" fill="#228b22"/>
                                            <circle cx="230" cy="200" r="3" fill="#228b22"/>
                                            <circle cx="150" cy="240" r="3" fill="#228b22"/>
                                            <circle cx="70" cy="200" r="3" fill="#228b22"/>
                                            <circle cx="70" cy="100" r="3" fill="#228b22"/>
                                            <line x1="150" y1="30" x2="150" y2="270" stroke="#e5e5e5" stroke-width="1" stroke-dasharray="4,4"/>
                                            <line x1="40" y1="150" x2="260" y2="150" stroke="#e5e5e5" stroke-width="1" stroke-dasharray="4,4"/>
                                            <text x="150" y="20" text-anchor="middle" font-size="11" fill="#4b5054">Returns</text>
                                            <text x="272" y="105" font-size="11" fill="#4b5054">Governance</text>
                                            <text x="272" y="215" font-size="11" fill="#4b5054">ESG</text>
                                            <text x="150" y="285" text-anchor="middle" font-size="11" fill="#4b5054">Risk Mgmt</text>
                                            <text x="20" y="215" font-size="11" fill="#4b5054">Fees</text>
                                            <text x="20" y="105" font-size="11" fill="#4b5054">Liquidity</text>
                                        </svg>
                                    </div>
                                </div>

                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 12px 0">Fund Description</h3>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.7;margin:0">Al-Baraka Islamic Growth Fund is a Shari'ah-compliant equity fund focusing on ethical investments in technology, healthcare, and renewable energy sectors. The fund employs a growth-oriented strategy with strict ESG screening and comprehensive Shari'ah governance oversight. Investments are diversified across emerging and developed markets with a focus on sustainable long-term value creation. The fund's rigorous compliance framework ensures adherence to both AAOIFI Shari'ah standards and global ESG best practices, making it a leading choice for values-based institutional investors seeking competitive returns aligned with ethical principles.</p>
                                </div>
                            </div>

                            <div id="bm-detail-performance" class="bm-detail-panel">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Performance History</h3>
                                    <div style="display:flex;flex-direction:column;gap:14px">
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">2026 YTD</span><span style="font-weight:700;color:#228b22">+8.2%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:82%;background:#228b22;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">2025 Annual</span><span style="font-weight:700;color:#228b22">+14.7%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:74%;background:#228b22;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">2024 Annual</span><span style="font-weight:700;color:#228b22">+11.3%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:65%;background:#228b22;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">2023 Annual</span><span style="font-weight:700;color:#228b22">+9.8%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:55%;background:#228b22;border-radius:12px"></div></div></div>
                                    </div>
                                </div>
                                <div style="background:#fff;border-radius:16px;padding:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Sector Allocation</h3>
                                    <div style="display:flex;flex-direction:column;gap:12px">
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Technology</span><span style="font-weight:600;color:#000">35%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:35%;background:#313eb2;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Healthcare</span><span style="font-weight:600;color:#000">28%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:28%;background:#228b22;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Renewable Energy</span><span style="font-weight:600;color:#000">22%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:22%;background:#ca8a04;border-radius:12px"></div></div></div>
                                        <div><div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="font-weight:600;color:#000">Consumer Staples</span><span style="font-weight:600;color:#000">15%</span></div><div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:15%;background:#4f46e5;border-radius:12px"></div></div></div>
                                    </div>
                                </div>
                            </div>

                            <div id="bm-detail-competitive" class="bm-detail-panel">
                                <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 16px 0">Peer Comparison</h3>
                                    <table style="width:100%;border-collapse:collapse;font-size:14px">
                                        <thead>
                                            <tr style="background:#f9fafb;border-bottom:1px solid #e5e5e5">
                                                <th style="padding:10px 14px;text-align:left;font-weight:600;color:#4b5054">Metric</th>
                                                <th style="padding:10px 14px;text-align:left;font-weight:600;color:#4b5054">This Fund</th>
                                                <th style="padding:10px 14px;text-align:left;font-weight:600;color:#4b5054">Peer Avg</th>
                                                <th style="padding:10px 14px;text-align:left;font-weight:600;color:#4b5054">Quartile</th>
                                            </tr>
                                        </thead>
                                        <tbody>
                                            <tr style="border-bottom:1px solid #f0f0f0"><td style="padding:10px 14px;color:#000;font-weight:500">1Y Return</td><td style="padding:10px 14px;color:#228b22;font-weight:600">12.5%</td><td style="padding:10px 14px;color:#4b5054">11.0%</td><td style="padding:10px 14px"><span style="padding:2px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Top Quartile</span></td></tr>
                                            <tr style="border-bottom:1px solid #f0f0f0"><td style="padding:10px 14px;color:#000;font-weight:500">3Y Return</td><td style="padding:10px 14px;color:#228b22;font-weight:600">32.5%</td><td style="padding:10px 14px;color:#4b5054">31.0%</td><td style="padding:10px 14px"><span style="padding:2px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Top Quartile</span></td></tr>
                                            <tr style="border-bottom:1px solid #f0f0f0"><td style="padding:10px 14px;color:#000;font-weight:500">5Y Return</td><td style="padding:10px 14px;color:#228b22;font-weight:600">62.5%</td><td style="padding:10px 14px;color:#4b5054">61.0%</td><td style="padding:10px 14px"><span style="padding:2px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Top Quartile</span></td></tr>
                                            <tr style="border-bottom:1px solid #f0f0f0"><td style="padding:10px 14px;color:#000;font-weight:500">Governance Score</td><td style="padding:10px 14px;color:#228b22;font-weight:600">96</td><td style="padding:10px 14px;color:#4b5054">65</td><td style="padding:10px 14px"><span style="padding:2px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Top Quartile</span></td></tr>
                                            <tr><td style="padding:10px 14px;color:#000;font-weight:500">ESG Score</td><td style="padding:10px 14px;color:#228b22;font-weight:600">88</td><td style="padding:10px 14px;color:#4b5054">82</td><td style="padding:10px 14px"><span style="padding:2px 10px;border-radius:8px;font-size:12px;font-weight:600;background:#eff6ff;color:#313eb2">2nd Quartile</span></td></tr>
                                        </tbody>
                                    </table>
                                </div>
                                <div style="background:#fff;border-radius:16px;padding:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                    <h3 style="font-size:18px;font-weight:700;color:#000;margin:0 0 12px 0">Competitive Positioning</h3>
                                    <p style="font-size:15px;color:#4b5054;line-height:1.7;margin:0">Al-Baraka Islamic Growth Fund maintains a strong competitive position within the Shari'ah-compliant equity space, consistently outperforming peer averages across all return periods. The fund's top-quartile governance score of 96 reflects its robust compliance framework and adherence to AAOIFI standards. Its ESG score of 88 places it in the 2nd quartile, indicating strong sustainability practices with room for improvement in environmental impact disclosure. The fund's differentiated focus on technology and renewable energy sectors provides a unique value proposition compared to conventional Islamic equity funds.</p>
                                </div>
                            </div>
                        </div>

                        <div>
                            <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Quick Stats</h3>
                                <div style="margin-bottom:14px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">Governance Score</span><span style="font-weight:700;color:#000">96</span></div>
                                    <div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:96%;background:#228b22;border-radius:12px"></div></div>
                                </div>
                                <div style="margin-bottom:16px">
                                    <div style="display:flex;justify-content:space-between;font-size:14px;margin-bottom:4px"><span style="color:#4b5054">ESG Score</span><span style="font-weight:700;color:#000">88%</span></div>
                                    <div style="width:100%;height:8px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:88%;background:#228b22;border-radius:12px"></div></div>
                                </div>
                                <div style="padding-top:16px;border-top:1px solid #e5e5e5">
                                    <h4 style="font-size:14px;font-weight:700;color:#000;margin:0 0 12px 0">Fee Structure</h4>
                                    <div style="display:flex;flex-direction:column;gap:8px">
                                        <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">Management</span><span style="font-weight:600;color:#000">1.2%</span></div>
                                        <div style="display:flex;justify-content:space-between;font-size:14px"><span style="color:#4b5054">Performance</span><span style="font-weight:600;color:#000">15%</span></div>
                                    </div>
                                </div>
                            </div>

                            <div style="background:#fff;border-radius:16px;padding:24px;margin-bottom:20px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Supporting Documents</h3>
                                <div style="display:flex;flex-direction:column;gap:10px">
                                    <div style="display:flex;align-items:center;gap:12px;background:#f9fafb;border-radius:10px;padding:12px 14px">
                                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                        <div style="flex:1;min-width:0"><div style="font-size:14px;font-weight:600;color:#000;white-space:nowrap;overflow:hidden;text-overflow:ellipsis">Market Analysis Report.pdf</div><div style="font-size:12px;color:#4b5054">2.4 MB</div></div>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer;flex-shrink:0"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                    </div>
                                    <div style="display:flex;align-items:center;gap:12px;background:#f9fafb;border-radius:10px;padding:12px 14px">
                                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                        <div style="flex:1;min-width:0"><div style="font-size:14px;font-weight:600;color:#000;white-space:nowrap;overflow:hidden;text-overflow:ellipsis">ESG Performance Overview Q1 2026.xlsx</div><div style="font-size:12px;color:#4b5054">1.8 MB</div></div>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer;flex-shrink:0"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                    </div>
                                    <div style="display:flex;align-items:center;gap:12px;background:#f9fafb;border-radius:10px;padding:12px 14px">
                                        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                        <div style="flex:1;min-width:0"><div style="font-size:14px;font-weight:600;color:#000;white-space:nowrap;overflow:hidden;text-overflow:ellipsis">Shari'ah Compliance Certificate.pdf</div><div style="font-size:12px;color:#4b5054">0.6 MB</div></div>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer;flex-shrink:0"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                    </div>
                                </div>
                            </div>

                            <div style="background:#fff;border-radius:16px;padding:24px;box-shadow:0 1px 3px rgba(0,0,0,0.05)">
                                <h3 style="font-size:16px;font-weight:700;color:#000;margin:0 0 16px 0">Actions</h3>
                                <div style="display:flex;flex-direction:column;gap:10px">
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#228b22;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><line x1="12" y1="8" x2="12" y2="16"/><line x1="8" y1="12" x2="16" y2="12"/></svg>
                                        Add to Comparison
                                    </button>
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#313eb2;color:#fff;border:none;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 12v8a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2v-8"/><polyline points="16 6 12 2 8 6"/><line x1="12" y1="2" x2="12" y2="15"/></svg>
                                        Share Report
                                    </button>
                                    <button style="display:flex;align-items:center;justify-content:center;gap:8px;width:100%;padding:12px;background:#fff;color:#000;border:1px solid #e5e5e5;border-radius:10px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21l-7-5-7 5V5a2 2 0 0 1 2-2h10a2 2 0 0 1 2 2z"/></svg>
                                        Save to Wishlist
                                    </button>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div id="bm-add-data" class="ra-view" style="display:none;background:#f5f5f5;min-height:100%;padding:0">
                <div style="max-width:1360px;margin:0 auto;padding:0">

                    <div style="display:flex;align-items:center;justify-content:space-between;padding:20px 30px">
                        <div style="display:flex;align-items:center;gap:16px">
                            <div @click="showBmAddDataBack()" style="width:40px;height:40px;border-radius:8px;border:1px solid #e5e5e5;display:flex;align-items:center;justify-content:center;cursor:pointer;background:#fff">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="15 18 9 12 15 6"/></svg>
                            </div>
                            <div>
                                <div style="font-size:28px;font-weight:700;color:#2d3643">Add Benchmark Data</div>
                                <div style="font-size:15px;color:#4b5054;margin-top:4px">Upload and document peer fund performance metrics</div>
                            </div>
                        </div>
                        <div style="display:flex;align-items:center;gap:12px">
                            <button @click="showBmAddDataBack()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:15px;font-weight:600;color:#2d3643;cursor:pointer;font-family:inherit">
                                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                                Save Draft
                            </button>
                            <button @click="submitBmBenchmarkData()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;background:#228b22;color:#fff;border:none;border-radius:8px;font-size:15px;font-weight:600;cursor:pointer;font-family:inherit">
                                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                                Submit for Review
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
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Fund Name*</label>
                                <input type="text" placeholder="Enter Peer fund name" style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none" />
                            </div>

                            <div style="display:grid;grid-template-columns:1fr 1fr;gap:16px;margin-bottom:16px">
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Fund Type*</label>
                                    <div style="display:flex;align-items:center;justify-content:space-between;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer;font-size:14px;color:#2d3643">
                                        <span>Ethical Fund</span>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                                    </div>
                                </div>
                                <div>
                                    <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Structure*</label>
                                    <div style="display:flex;align-items:center;justify-content:space-between;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;cursor:pointer;font-size:14px;color:#2d3643">
                                        <span>Mudarabah</span>
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#4b5054" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                                    </div>
                                </div>
                            </div>

                            <div style="display:flex;align-items:center;gap:8px;margin-bottom:20px">
                                <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                                <span style="font-size:14px;color:#228b22;font-weight:600">Shari'ah Compliant</span>
                            </div>

                            <div>
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Assets Under Management</label>
                                <input type="text" placeholder="e.g., $450M" style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none" />
                            </div>

                            <div style="height:1px;background:#e5e5e5;margin:24px 0"></div>

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M12 20V10"/><path d="M18 20V4"/><path d="M6 20v-6"/></svg>
                                Performance Metrics
                            </div>
                            <div style="height:1px;background:#e5e5e5;margin-bottom:20px"></div>

                            <div style="margin-bottom:24px">
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">Governance Score: <span id="bm-gov-score-val">0</span>/100</span>
                                </div>
                                <input type="range" min="0" max="100" value="0" oninput="document.getElementById('bm-gov-score-val').textContent=this.value" style="width:100%;-webkit-appearance:none;height:6px;border-radius:3px;background:linear-gradient(to right, #d1d5db 0%, #60a5fa 50%, #3b82f6 100%);outline:none" />
                                <div style="display:flex;justify-content:space-between;font-size:12px;color:#4b5054;margin-top:4px">
                                    <span>Poor (0)</span>
                                    <span>Fair (50)</span>
                                    <span>Excellent (100)</span>
                                </div>
                            </div>

                            <div style="margin-bottom:24px">
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:8px">
                                    <span style="font-size:14px;font-weight:600;color:#2d3643">ESG Score: <span id="bm-esg-score-val">0</span>/100</span>
                                </div>
                                <input type="range" min="0" max="100" value="0" oninput="document.getElementById('bm-esg-score-val').textContent=this.value" style="width:100%;-webkit-appearance:none;height:6px;border-radius:3px;background:linear-gradient(to right, #d1d5db 0%, #60a5fa 50%, #3b82f6 100%);outline:none" />
                                <div style="display:flex;justify-content:space-between;font-size:12px;color:#4b5054;margin-top:4px">
                                    <span>Poor (0)</span>
                                    <span>Fair (50)</span>
                                    <span>Excellent (100)</span>
                                </div>
                            </div>

                            <div style="height:1px;background:#e5e5e5;margin:24px 0"></div>

                            <div style="display:flex;align-items:center;gap:8px;font-size:16px;font-weight:700;color:#2d3643;margin-bottom:16px">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><polyline points="14 2 14 8 20 8"/><line x1="16" y1="13" x2="8" y2="13"/><line x1="16" y1="17" x2="8" y2="17"/><polyline points="10 9 9 9 8 9"/></svg>
                                Qualitative Analysis
                            </div>
                            <div style="height:1px;background:#e5e5e5;margin-bottom:20px"></div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Fund Description</label>
                                <textarea rows="4" placeholder="Analyze the macroeconomic factors, market trends and potential impact..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
                            </div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Key Strengths</label>
                                <textarea rows="3" placeholder="Analyze the macroeconomic factors, market trends and potential impact..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
                            </div>

                            <div style="margin-bottom:16px">
                                <label style="display:block;font-size:14px;font-weight:600;color:#2d3643;margin-bottom:6px">Key Weaknesses</label>
                                <textarea rows="3" placeholder="Analyze the macroeconomic factors, market trends and potential impact..." style="width:100%;padding:12px 14px;border:1px solid #e5e5e5;border-radius:8px;font-size:14px;font-family:inherit;outline:none;resize:vertical"></textarea>
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
                                    <button @click="showBmAddDataBack()" style="display:flex;align-items:center;gap:6px;padding:8px 16px;background:transparent;border:none;font-size:15px;color:#4b5054;cursor:pointer;font-family:inherit">
                                        <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="18" y1="6" x2="6" y2="18"/><line x1="6" y1="6" x2="18" y2="18"/></svg>
                                        Cancel
                                    </button>
                                </div>
                                <div style="display:flex;align-items:center;gap:12px">
                                    <button @click="showBmAddDataBack()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:15px;font-weight:600;color:#2d3643;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                                        Save Draft
                                    </button>
                                    <button @click="submitBmBenchmarkData()" style="display:flex;align-items:center;gap:8px;padding:10px 20px;background:#228b22;color:#fff;border:none;border-radius:8px;font-size:15px;font-weight:600;cursor:pointer;font-family:inherit">
                                        <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                                        Submit Benchmark Data
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




</template>
<script setup>
import { ref } from "vue";
const showBmAddData = (...args) => { console.log('showBmAddData called', args); };
const showBmDetail = (...args) => { console.log('showBmDetail called', args); };
const showBmList = (...args) => { console.log('showBmList called', args); };
const switchBmDetailTab = (...args) => { console.log('switchBmDetailTab called', args); };
const showBmAddDataBack = (...args) => { console.log('showBmAddDataBack called', args); };
const submitBmBenchmarkData = (...args) => { console.log('submitBmBenchmarkData called', args); };
</script>