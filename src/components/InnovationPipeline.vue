<template>
<div>
            <div style="background:#fff;padding:20px 30px 16px">
                <div style="display:flex;justify-content:space-between;align-items:center">
                    <div>
                        <h1 style="font-size:24px;font-weight:700;color:#2d3643">Innovation Pipeline</h1>
                        <p style="font-size:20px;color:#2d3643;margin-top:4px">Track and manage new product and instrument ideas</p>
                    </div>
                    <div style="display:flex;gap:12px;align-items:center">
                        <div style="width:41px;height:41px;background:#fff;border:1px solid #e5e5e5;border-radius:13px;display:flex;align-items:center;justify-content:center;cursor:pointer;position:relative">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><path d="M9.09 9a3 3 0 0 1 5.83 1c0 2-3 3-3 3"/><path d="M12 17h.01"/></svg>
                        </div>
                        <div style="width:41px;height:41px;background:#fff;border:1px solid #e5e5e5;border-radius:13px;display:flex;align-items:center;justify-content:center;cursor:pointer;position:relative">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M18 8A6 6 0 0 0 6 8c0 7-3 9-3 9h18s-3-2-3-9"/><path d="M13.73 21a2 2 0 0 1-3.46 0"/></svg>
                            <span style="position:absolute;top:-2px;right:-4px;width:15px;height:15px;background:#fa0000;border-radius:50%;font-size:10px;font-weight:600;color:#fff;display:flex;align-items:center;justify-content:center">0</span>
                        </div>
                        <button id="ip-submit-new-idea-btn" style="display:flex;align-items:center;gap:8px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:12px 20px;font-family:inherit;font-size:16px;cursor:pointer">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                            Submit New Idea
                        </button>
                    </div>
                </div>
            </div>
            <div style="background:#fff;padding:0 30px;display:flex;gap:0;border-bottom:1px solid #e5e5e5">
                <div class="ip-tab-item active" data-ip-tab="kanban" style="display:flex;align-items:center;gap:8px;padding:14px 24px;font-size:16px;cursor:pointer;position:relative;color:#228b22;font-weight:600">
                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="7" height="7"/><rect x="14" y="3" width="7" height="7"/><rect x="14" y="14" width="7" height="7"/><rect x="3" y="14" width="7" height="7"/></svg>
                    Kanban Board
                </div>
                <div class="ip-tab-item" data-ip-tab="list" style="display:flex;align-items:center;gap:8px;padding:14px 24px;font-size:16px;cursor:pointer;position:relative;color:#000">
                    <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="3" y1="6" x2="21" y2="6"/><line x1="3" y1="12" x2="21" y2="12"/><line x1="3" y1="18" x2="21" y2="18"/></svg>
                    List View
                </div>
            </div>
            <div id="ip-tab-kanban" class="ip-tab-panel active">
                <div style="display:flex;gap:16px;padding:16px 30px">
                    <div style="flex:1;border-radius:12px;padding:20px 24px;background:#228b22;color:#fff"><div style="font-size:32px;font-weight:600">6</div><div style="font-size:16px;font-weight:600;margin-top:8px">Total Ideas</div></div>
                    <div style="flex:1;border-radius:12px;padding:20px 24px;background:#313eb2;color:#fff"><div style="font-size:32px;font-weight:600">6</div><div style="font-size:16px;font-weight:600;margin-top:8px">In Progress</div></div>
                    <div style="flex:1;border-radius:12px;padding:20px 24px;background:#e50303;color:#fff"><div style="font-size:32px;font-weight:600">6</div><div style="font-size:16px;font-weight:600;margin-top:8px">Pending Approval</div></div>
                    <div style="flex:1;border-radius:12px;padding:20px 24px;background:#4b5054;color:#fff"><div style="font-size:32px;font-weight:600">76%</div><div style="font-size:16px;font-weight:600;margin-top:8px">Avg. Score</div></div>
                </div>
                <div style="display:flex;gap:8px;padding:16px 30px 30px;overflow-x:auto">
                    <div style="width:367px;flex-shrink:0;background:#f9fafb;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;gap:8px;margin-bottom:16px">
                            <span style="font-size:16px;font-weight:600;color:#4b5054">Idea Log</span>
                            <span style="width:24px;height:24px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600">1</span>
                            <button style="margin-left:auto;background:none;border:none;cursor:pointer;width:24px;height:24px;color:#4b5054"><svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/></svg></button>
                            <button style="background:none;border:none;cursor:pointer;font-size:20px;color:#4b5054">⋮</button>
                        </div>
                        <div class="ip-card-click" style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;margin-bottom:12px;display:flex;overflow:hidden">
                            <div style="width:6px;background:#228b22;flex-shrink:0"></div>
                            <div style="padding:14px 16px;flex:1;min-width:0">
                                <div style="display:flex;align-items:flex-start;gap:8px;margin-bottom:8px">
                                    <div style="width:31px;height:35px;background:#228b22;border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg width="16" height="16" viewBox="0 0 16 16" fill="none" stroke="#fff" stroke-width="1.5"><rect x="2" y="4" width="12" height="10" rx="1"/><path d="M5 4V2h6v2"/></svg></div>
                                    <h4 style="font-size:16px;font-weight:600;color:#000;flex:1">Healthcare Innovation PE Fund</h4>
                                    <span style="font-size:12px;padding:4px 10px;border-radius:8px;background:#e5e5e5">Pending</span>
                                    <button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋯</button>
                                </div>
                                <p style="font-size:12px;color:#000;line-height:1.4;margin-bottom:10px">Private equity fund investing in healthcare technology and medical devices</p>
                                <span style="display:inline-block;font-size:12px;color:#fff;background:#228b22;border-radius:4px;padding:6px 10px;margin-bottom:12px">Private Equity</span>
                                <div style="border-top:1px solid #e5e5e5;margin-bottom:10px"></div>
                                <div style="display:flex;align-items:center;gap:8px">
                                    <div style="width:27px;height:27px;border-radius:50%;background:#ccc;flex-shrink:0"></div>
                                    <span style="font-size:12px;color:#000">Fatima Khan</span>
                                    <span style="font-size:12px;color:#4b5054;margin-left:auto">1/22/2025</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div style="width:367px;flex-shrink:0;background:#f9fafb;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;gap:8px;margin-bottom:16px">
                            <span style="font-size:16px;font-weight:600;color:#4b5054">Scoring</span>
                            <span style="width:24px;height:24px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600">1</span>
                            <button style="margin-left:auto;background:none;border:none;cursor:pointer;width:24px;height:24px;color:#4b5054"><svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/></svg></button>
                            <button style="background:none;border:none;cursor:pointer;font-size:20px;color:#4b5054">⋮</button>
                        </div>
                        <div class="ip-card-click" style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;margin-bottom:12px;display:flex;overflow:hidden">
                            <div style="width:6px;background:#228b22;flex-shrink:0"></div>
                            <div style="padding:14px 16px;flex:1;min-width:0">
                                <div style="display:flex;align-items:flex-start;gap:8px;margin-bottom:8px">
                                    <div style="width:31px;height:35px;background:#228b22;border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg width="16" height="16" viewBox="0 0 16 16" fill="none" stroke="#fff" stroke-width="1.5"><rect x="2" y="4" width="12" height="10" rx="1"/><path d="M5 4V2h6v2"/></svg></div>
                                    <h4 style="font-size:16px;font-weight:600;color:#000;flex:1">Healthcare Innovation PE Fund</h4>
                                    <span style="font-size:12px;padding:4px 10px;border-radius:8px;background:#e5e5e5">Pending</span>
                                    <button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋯</button>
                                </div>
                                <p style="font-size:12px;color:#000;line-height:1.4;margin-bottom:10px">Private equity fund investing in healthcare technology and medical devices</p>
                                <span style="display:inline-block;font-size:12px;color:#fff;background:#228b22;border-radius:4px;padding:6px 10px;margin-bottom:12px">Private Equity</span>
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px"><span style="font-size:12px;color:#000">Overall Score</span><span style="font-size:14px;font-weight:600;color:#eff31c">71%</span></div>
                                <div style="width:100%;height:11px;background:#d9d9d9;border-radius:12px;overflow:hidden;margin-bottom:12px"><div style="height:11px;border-radius:12px;width:71%;background:#228b22"></div></div>
                                <div style="border-top:1px solid #e5e5e5;margin-bottom:10px"></div>
                                <div style="display:flex;align-items:center;gap:8px">
                                    <div style="width:27px;height:27px;border-radius:50%;background:#ccc;flex-shrink:0"></div>
                                    <span style="font-size:12px;color:#000">Fatima Khan</span>
                                    <span style="font-size:12px;color:#4b5054;margin-left:auto">1/22/2025</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div style="width:367px;flex-shrink:0;background:#f9fafb;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;gap:8px;margin-bottom:16px">
                            <span style="font-size:16px;font-weight:600;color:#4b5054">Evaluation</span>
                            <span style="width:24px;height:24px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600">2</span>
                            <button style="margin-left:auto;background:none;border:none;cursor:pointer;width:24px;height:24px;color:#4b5054"><svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/></svg></button>
                            <button style="background:none;border:none;cursor:pointer;font-size:20px;color:#4b5054">⋮</button>
                        </div>
                        <div class="ip-card-click" style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;margin-bottom:12px;display:flex;overflow:hidden">
                            <div style="width:6px;background:#228b22;flex-shrink:0"></div>
                            <div style="padding:14px 16px;flex:1;min-width:0">
                                <div style="display:flex;align-items:flex-start;gap:8px;margin-bottom:8px">
                                    <div style="width:31px;height:35px;background:#228b22;border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg width="16" height="16" viewBox="0 0 16 16" fill="none" stroke="#fff" stroke-width="1.5"><rect x="2" y="4" width="12" height="10" rx="1"/><path d="M5 4V2h6v2"/></svg></div>
                                    <h4 style="font-size:16px;font-weight:600;color:#000;flex:1">Healthcare Innovation PE Fund</h4>
                                    <span style="font-size:12px;padding:4px 10px;border-radius:8px;background:#eff31c">In progress</span>
                                    <button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋯</button>
                                </div>
                                <p style="font-size:12px;color:#000;line-height:1.4;margin-bottom:10px">Private equity fund investing in healthcare technology and medical devices</p>
                                <span style="display:inline-block;font-size:12px;color:#fff;background:#228b22;border-radius:4px;padding:6px 10px;margin-bottom:12px">Private Equity</span>
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px"><span style="font-size:12px;color:#000">Overall Score</span><span style="font-size:14px;font-weight:600;color:#228b22">71%</span></div>
                                <div style="width:100%;height:11px;background:#d9d9d9;border-radius:12px;overflow:hidden;margin-bottom:12px"><div style="height:11px;border-radius:12px;width:71%;background:#228b22"></div></div>
                                <div style="border-top:1px solid #e5e5e5;margin-bottom:10px"></div>
                                <div style="display:flex;align-items:center;gap:8px">
                                    <div style="width:27px;height:27px;border-radius:50%;background:#ccc;flex-shrink:0"></div>
                                    <span style="font-size:12px;color:#000">Fatima Khan</span>
                                    <span style="font-size:12px;color:#4b5054;margin-left:auto">1/22/2025</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div style="width:367px;flex-shrink:0;background:#f9fafb;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;gap:8px;margin-bottom:16px">
                            <span style="font-size:16px;font-weight:600;color:#4b5054">Prototype</span>
                            <span style="width:24px;height:24px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600">2</span>
                            <button style="margin-left:auto;background:none;border:none;cursor:pointer;width:24px;height:24px;color:#4b5054"><svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/></svg></button>
                            <button style="background:none;border:none;cursor:pointer;font-size:20px;color:#4b5054">⋮</button>
                        </div>
                        <div class="ip-card-click" style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;margin-bottom:12px;display:flex;overflow:hidden">
                            <div style="width:6px;background:#228b22;flex-shrink:0"></div>
                            <div style="padding:14px 16px;flex:1;min-width:0">
                                <div style="display:flex;align-items:flex-start;gap:8px;margin-bottom:8px">
                                    <div style="width:31px;height:35px;background:#228b22;border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg width="16" height="16" viewBox="0 0 16 16" fill="none" stroke="#fff" stroke-width="1.5"><rect x="2" y="4" width="12" height="10" rx="1"/><path d="M5 4V2h6v2"/></svg></div>
                                    <h4 style="font-size:16px;font-weight:600;color:#000;flex:1">Healthcare Innovation PE Fund</h4>
                                    <span style="font-size:12px;padding:4px 10px;border-radius:8px;background:#eff31c">In progress</span>
                                    <button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋯</button>
                                </div>
                                <p style="font-size:12px;color:#000;line-height:1.4;margin-bottom:10px">Private equity fund investing in healthcare technology and medical devices</p>
                                <span style="display:inline-block;font-size:12px;color:#fff;background:#228b22;border-radius:4px;padding:6px 10px;margin-bottom:12px">Private Equity</span>
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px"><span style="font-size:12px;color:#000">Overall Score</span><span style="font-size:14px;font-weight:600;color:#228b22">71%</span></div>
                                <div style="width:100%;height:11px;background:#d9d9d9;border-radius:12px;overflow:hidden;margin-bottom:12px"><div style="height:11px;border-radius:12px;width:71%;background:#228b22"></div></div>
                                <div style="border-top:1px solid #e5e5e5;margin-bottom:10px"></div>
                                <div style="display:flex;align-items:center;gap:8px">
                                    <div style="width:27px;height:27px;border-radius:50%;background:#ccc;flex-shrink:0"></div>
                                    <span style="font-size:12px;color:#000">Fatima Khan</span>
                                    <span style="font-size:12px;color:#4b5054;margin-left:auto">1/22/2025</span>
                                </div>
                            </div>
                        </div>
                    </div>
                    <div style="width:367px;flex-shrink:0;background:#f9fafb;border-radius:12px;padding:16px">
                        <div style="display:flex;align-items:center;gap:8px;margin-bottom:16px">
                            <span style="font-size:16px;font-weight:600;color:#4b5054">Approval</span>
                            <span style="width:24px;height:24px;background:#fff;border-radius:9px;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600">2</span>
                            <button style="margin-left:auto;background:none;border:none;cursor:pointer;width:24px;height:24px;color:#4b5054"><svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor"><path d="M19 11h-6V5a1 1 0 0 0-2 0v6H5a1 1 0 0 0 0 2h6v6a1 1 0 0 0 2 0v-6h6a1 1 0 0 0 0-2z"/></svg></button>
                            <button style="background:none;border:none;cursor:pointer;font-size:20px;color:#4b5054">⋮</button>
                        </div>
                        <div class="ip-card-click" style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;margin-bottom:12px;display:flex;overflow:hidden">
                            <div style="width:6px;background:#228b22;flex-shrink:0"></div>
                            <div style="padding:14px 16px;flex:1;min-width:0">
                                <div style="display:flex;align-items:flex-start;gap:8px;margin-bottom:8px">
                                    <div style="width:31px;height:35px;background:#228b22;border-radius:4px;display:flex;align-items:center;justify-content:center;flex-shrink:0"><svg width="16" height="16" viewBox="0 0 16 16" fill="none" stroke="#fff" stroke-width="1.5"><rect x="2" y="4" width="12" height="10" rx="1"/><path d="M5 4V2h6v2"/></svg></div>
                                    <h4 style="font-size:16px;font-weight:600;color:#000;flex:1">Healthcare Innovation PE Fund</h4>
                                    <span style="font-size:12px;padding:4px 10px;border-radius:8px;background:#eff31c">In progress</span>
                                    <button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋯</button>
                                </div>
                                <p style="font-size:12px;color:#000;line-height:1.4;margin-bottom:10px">Private equity fund investing in healthcare technology and medical devices</p>
                                <span style="display:inline-block;font-size:12px;color:#fff;background:#228b22;border-radius:4px;padding:6px 10px;margin-bottom:12px">Private Equity</span>
                                <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:6px"><span style="font-size:12px;color:#000">Overall Score</span><span style="font-size:14px;font-weight:600;color:#228b22">71%</span></div>
                                <div style="width:100%;height:11px;background:#d9d9d9;border-radius:12px;overflow:hidden;margin-bottom:12px"><div style="height:11px;border-radius:12px;width:71%;background:#228b22"></div></div>
                                <div style="border-top:1px solid #e5e5e5;margin-bottom:10px"></div>
                                <div style="display:flex;align-items:center;gap:8px">
                                    <div style="width:27px;height:27px;border-radius:50%;background:#ccc;flex-shrink:0"></div>
                                    <span style="font-size:12px;color:#000">Fatima Khan</span>
                                    <span style="font-size:12px;color:#4b5054;margin-left:auto">1/22/2025</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
            <div id="ip-tab-list" class="ip-tab-panel">
                <div style="display:flex;align-items:center;justify-content:space-between;padding:16px 30px;gap:12px">
                    <div style="display:flex;align-items:center;gap:8px">
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polygon points="22 3 2 3 10 12.46 10 19 14 21 14 12.46 22 3"/></svg>
                            Filter
                        </div>
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="4" y1="6" x2="20" y2="6"/><line x1="6" y1="12" x2="18" y2="12"/><line x1="8" y1="18" x2="16" y2="18"/></svg>
                            Sort
                        </div>
                    </div>
                    <div style="display:flex;align-items:center;gap:12px">
                        <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;font-weight:600;color:#4b5054;cursor:pointer">
                            View: My Pipeline
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                        </div>
                        <div style="font-size:14px;color:#4b5054">24 opportunities</div>
                    </div>
                </div>
                <div style="margin:0 30px 30px;background:#fff;border-radius:12px;overflow:hidden">
                    <div style="display:flex;align-items:center;justify-content:space-between;padding:16px 24px;border-bottom:1px solid #e5e5e5">
                        <div>
                            <div style="font-size:18px;font-weight:700;color:#000">Pipeline Tracker</div>
                            <div style="font-size:14px;color:#4b5054;margin-top:2px">Central repository of all innovation opportunities</div>
                        </div>
                        <div style="display:flex;align-items:center;gap:8px">
                            <div style="display:flex;align-items:center;gap:8px;padding:8px 16px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:14px;color:#000;cursor:pointer">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                Export
                            </div>
                            <button style="display:flex;align-items:center;gap:8px;padding:8px 16px;background:#228b22;color:#fff;border:none;border-radius:8px;font-family:inherit;font-size:14px;font-weight:600;cursor:pointer">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                                Add Opportunity
                            </button>
                        </div>
                    </div>
                    <table style="width:100%;border-collapse:collapse">
                        <thead>
                            <tr>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Lead Name</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Contact</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Stage</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Probability</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Value</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Sector</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Owner</th>
                                <th style="text-align:left;padding:12px 16px;font-size:12px;font-weight:600;color:#4b5054;background:#e5e5e5;text-transform:uppercase">Action</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">Global Tech Solutions</div><div style="font-size:12px;color:#4b5054;margin-top:2px">International Growth</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">j.anderson@techcorp.com</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8123456789</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Active</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:68%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">68%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦1.6M</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#e5e5e5;color:#4b5054">Technology</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">James Anderson</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">AfriGreen Energy Ltd</div><div style="font-size:12px;color:#4b5054;margin-top:2px">Renewable Energy</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">s.okonkwo@afrigreen.com</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8098765432</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Proposal</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:52%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">52%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦2.8M</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#dcfce7;color:#228b22">Energy</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">Sarah Okonkwo</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">FinServe Africa</div><div style="font-size:12px;color:#4b5054;margin-top:2px">Digital Banking</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">a.adeyemi@finserve.ng</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8056781234</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#fef9c3;color:#946325">Negotiation</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:78%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">78%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦3.2M</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#eff6ff;color:#313eb2">Financial Services</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">Amaka Adeyemi</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">HealthBridge Pharma</div><div style="font-size:12px;color:#4b5054;margin-top:2px">Medical Devices</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">d.ibrahim@healthbridge.com</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8034567890</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#f3f4f6;color:#4b5054">Outreach</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:35%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">35%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦900K</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#fee2e2;color:#e50303">Healthcare</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">Dr. Ibrahim</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">AgriTech Solutions</div><div style="font-size:12px;color:#4b5054;margin-top:2px">Smart Farming</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">c.nwosu@agritech.ng</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8076543210</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#dcfce7;color:#228b22">Conversion</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:88%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">88%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦1.2M</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#dcfce7;color:#228b22">Agriculture</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">Chioma Nwosu</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                            <tr class="ip-row-click">
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:14px;font-weight:600;color:#000">EduPrime Technologies</div><div style="font-size:12px;color:#4b5054;margin-top:2px">E-Learning</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="font-size:12px;color:#4b5054">t.bello@eduprime.com</div><div style="font-size:12px;color:#4b5054;margin-top:1px">(+234) 8012345678</div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 12px;border-radius:12px;font-size:12px;font-weight:600;background:#f3f4f6;color:#4b5054">Prospect</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><div style="display:flex;align-items:center;gap:8px"><div style="width:60px;height:6px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:100%;width:22%;background:#228b22;border-radius:12px"></div></div><span style="font-size:12px;font-weight:600;color:#000">22%</span></div></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:14px;font-weight:600;color:#000">₦500K</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="display:inline-block;padding:4px 10px;border-radius:8px;font-size:12px;font-weight:500;background:#fef9c3;color:#946325">Education</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><span style="font-size:13px;color:#000">Tunde Bello</span></td>
                                <td style="padding:14px 16px;border-bottom:1px solid #e5e5e5"><button style="background:none;border:none;cursor:pointer;font-size:18px;color:#4b5054">⋮</button></td>
                            </tr>
                        </tbody>
                    </table>
                    <div style="display:flex;align-items:center;justify-content:space-between;padding:16px 24px;border-top:1px solid #e5e5e5">
                        <span style="font-size:13px;color:#000">Showing 1-6 of 24 opportunities</span>
                        <div style="display:flex;gap:6px">
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:13px;font-weight:600;color:#000;cursor:pointer;opacity:0.5">&lt;</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #228b22;border-radius:4px;background:#228b22;font-size:13px;font-weight:600;color:#fff;cursor:pointer">1</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:13px;font-weight:600;color:#000;cursor:pointer">2</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:13px;font-weight:600;color:#000;cursor:pointer">3</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:13px;font-weight:600;color:#000;cursor:pointer">4</button>
                            <button style="width:28px;height:28px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:13px;font-weight:600;color:#000;cursor:pointer">&gt;</button>
                        </div>
                    </div>
                </div>
            </div>


</div>
</template>
<script setup>
import { ref } from "vue";
</script>