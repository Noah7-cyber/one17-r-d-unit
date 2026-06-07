<template>
<div>

            <div class="mr-tabs-bar" style="background:#fff;height:68px;display:flex;align-items:center;padding:0 22px;gap:0">
                <div class="mr-tab-item active" data-mr-tab="research-list" style="display:flex;align-items:center;gap:8px;padding:12px 20px;font-size:16px;cursor:pointer;position:relative;color:#228b22;font-weight:600">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><rect x="3" y="3" width="18" height="18" rx="2"/><path d="M3 9h18"/><path d="M9 21V9"/></svg>
                    Research List
                    <span style="display:inline-flex;align-items:center;justify-content:center;padding:2px 10px;border-radius:12px;font-size:14px;min-width:27px;height:23px;background:#228b22;color:#fff">47</span>
                </div>
                <div class="mr-tab-item" data-mr-tab="new-brief" style="display:flex;align-items:center;gap:8px;padding:12px 20px;font-size:16px;cursor:pointer;position:relative;color:#000">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="12" y1="5" x2="12" y2="19"/><line x1="5" y1="12" x2="19" y2="12"/></svg>
                    New Brief
                </div>
                <div class="mr-tab-item" data-mr-tab="brief-detail" style="display:flex;align-items:center;gap:8px;padding:12px 20px;font-size:16px;cursor:pointer;position:relative;color:#000">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                    Brief Detail
                    <span style="display:inline-flex;align-items:center;justify-content:center;padding:2px 10px;border-radius:12px;font-size:14px;min-width:27px;height:23px;background:#e5e5e5;color:#0f151f">View</span>
                </div>
                <div class="mr-tab-item" data-mr-tab="approval-flow" style="display:flex;align-items:center;gap:8px;padding:12px 20px;font-size:16px;cursor:pointer;position:relative;color:#000">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M9 11l3 3L22 4"/><path d="M21 12v7a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11"/></svg>
                    Approval Flow
                    <span style="display:inline-flex;align-items:center;justify-content:center;padding:2px 10px;border-radius:12px;font-size:14px;min-width:27px;height:23px;background:#e5e5e5;color:#0f151f">3</span>
                </div>
                <div style="margin-left:auto">
                    <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
                </div>
            </div>

            <div id="mr-tab-research-list" class="mr-tab-panel active">
                <div style="display:flex;gap:20px;padding:22px 36px">
                    <div style="flex:1;background:#fff;border-radius:12px;padding:20px 22px">
                        <div style="font-size:24px;font-weight:600;color:#228b22">47</div>
                        <div style="font-size:16px;font-weight:600;color:#4b5054;margin:12px 0 8px">TOTAL BRIEFS</div>
                        <div style="font-size:12px;font-weight:600;color:#228b22">12% this quarter</div>
                    </div>
                    <div style="flex:1;background:#fff;border-radius:12px;padding:20px 22px">
                        <div style="font-size:24px;font-weight:600;color:#313eb2">12</div>
                        <div style="font-size:16px;font-weight:600;color:#000;margin:12px 0 8px">IN REVIEW</div>
                        <div style="font-size:12px;font-weight:600;color:#4b5054">3 pending action</div>
                    </div>
                    <div style="flex:1;background:#fff;border-radius:12px;padding:20px 22px">
                        <div style="font-size:24px;font-weight:600;color:#228b22">28</div>
                        <div style="font-size:16px;font-weight:600;color:#000;margin:12px 0 8px">APPROVED</div>
                        <div style="font-size:12px;font-weight:600;color:#228b22">+8 this month</div>
                    </div>
                    <div style="flex:1;background:#fff;border-radius:12px;padding:20px 22px">
                        <div style="font-size:24px;font-weight:600;color:#e50303">3</div>
                        <div style="font-size:16px;font-weight:600;color:#000;margin:12px 0 8px">FLAGGED/OVERDUE</div>
                        <div style="font-size:12px;font-weight:600;color:#e50303">Needs attention</div>
                    </div>
                </div>
                <div style="background:#fff;border-radius:12px;margin:0 36px 30px;overflow:hidden">
                    <div style="display:flex;align-items:center;justify-content:space-between;padding:20px 30px;border:1px solid #e5e5e5">
                        <div>
                            <div style="font-size:16px;font-weight:600;color:#000">Research Briefs Registry</div>
                            <div style="font-size:14px;color:#000;margin-top:4px">All analysts &middot; Filterable &middot; Exportable</div>
                        </div>
                        <div style="display:flex;gap:12px;align-items:center">
                            <div style="display:flex;align-items:center;gap:8px;background:#f5f5f5;border:1px solid #a5a5a8;border-radius:8px;padding:10px 12px;height:40px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#a5a5a8" stroke-width="2"><circle cx="11" cy="11" r="8"/><path d="m21 21-4.35-4.35"/></svg>
                                <input type="text" placeholder="Search ..." style="border:none;background:none;font-family:inherit;font-size:16px;font-weight:600;color:#a5a5a8;outline:none;width:100%" />
                            </div>
                            <div style="display:flex;align-items:center;justify-content:space-between;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:10px 12px;height:40px;min-width:140px;font-size:16px;font-weight:600;color:#4b5054;cursor:pointer">
                                All Status
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                            </div>
                            <div style="display:flex;align-items:center;justify-content:space-between;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:10px 12px;height:40px;min-width:140px;font-size:16px;font-weight:600;color:#4b5054;cursor:pointer">
                                All Sectors
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg>
                            </div>
                            <button style="display:flex;align-items:center;gap:10px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:10px 12px;height:40px;font-size:16px;font-weight:600;color:#4b5054;cursor:pointer;font-family:inherit">
                                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                                Export Report
                            </button>
                        </div>
                    </div>
                    <table style="width:100%;border-collapse:collapse;table-layout:fixed">
                        <thead>
                            <tr>
                                <th style="width:40px;text-align:center;background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054"><input type="checkbox" style="width:19px;height:19px;border:1px solid #e5e5e5;border-radius:4px;cursor:pointer;appearance:none" /></th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">TITLE</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">SECTOR</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">ANALYST</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">STATUS</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">COMPLETED</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">ALIGNMENT</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">SHARI'AH</th>
                                <th style="background:#e5e5e5;padding:16px 12px;font-size:13px;font-weight:400;color:#4b5054;text-align:left">ACTION</th>
                            </tr>
                        </thead>
                        <tbody>
                            <tr>
                                <td style="text-align:center;padding:16px 12px;border:1px solid #e5e5e5"><input type="checkbox" style="width:19px;height:19px;border:1px solid #e5e5e5;border-radius:4px;cursor:pointer;appearance:none" /></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="font-size:14px;font-weight:600;color:#000">Islamic FinTech Landscape</div><div style="font-size:12px;color:#4b5054;margin-top:4px">FinTech</div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;background:#e5e5e5;border-radius:8px;padding:4px 10px;font-size:13px;color:#4b5054">FINTECH</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="display:flex;align-items:center;gap:8px"><div style="width:37px;height:37px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600;color:#fff">AS</div>A. Suleiman</div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;padding:6px 10px;border-radius:12px;font-size:13px;font-weight:600;background:#228b22;color:#fff">APPROVED</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054">Feb 24</td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div>92</div><div style="width:59px;height:6px;background:#d9d9d9;border-radius:12px;position:relative"><div style="height:6px;border-radius:12px;position:absolute;top:0;left:0;width:78%;background:#228b22"></div></div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;padding:6px 10px;border-radius:12px;font-size:13px;font-weight:600;background:#228b22;border:1px solid #228b22;color:#fff">YES</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="display:flex;gap:4px"><button style="display:flex;align-items:center;gap:4px;padding:6px 10px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:13px;color:#4b5054;cursor:pointer;font-family:inherit"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"/><circle cx="12" cy="12" r="3"/></svg>View</button><button style="display:flex;align-items:center;gap:4px;padding:6px 10px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:13px;color:#4b5054;cursor:pointer;font-family:inherit"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg></button></div></td>
                            </tr>
                            <tr>
                                <td style="text-align:center;padding:16px 12px;border:1px solid #e5e5e5"><input type="checkbox" style="width:19px;height:19px;border:1px solid #e5e5e5;border-radius:4px;cursor:pointer;appearance:none" /></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="font-size:14px;font-weight:600;color:#000">Islamic FinTech Landscape</div><div style="font-size:12px;color:#4b5054;margin-top:4px">FinTech</div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;background:#e5e5e5;border-radius:8px;padding:4px 10px;font-size:13px;color:#4b5054">FINTECH</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="display:flex;align-items:center;gap:8px"><div style="width:37px;height:37px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;font-size:14px;font-weight:600;color:#fff">AS</div>A. Suleiman</div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;padding:6px 10px;border-radius:12px;font-size:13px;font-weight:600;background:#fef9c3;color:#92400e">PENDING</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054">Feb 24</td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div>92</div><div style="width:59px;height:6px;background:#d9d9d9;border-radius:12px;position:relative"><div style="height:6px;border-radius:12px;position:absolute;top:0;left:0;width:78%;background:#228b22"></div></div></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><span style="display:inline-block;padding:6px 10px;border-radius:12px;font-size:13px;font-weight:600;background:#228b22;border:1px solid #228b22;color:#fff">YES</span></td>
                                <td style="padding:16px 12px;border:1px solid #e5e5e5;font-size:13px;color:#4b5054"><div style="display:flex;gap:4px"><button style="display:flex;align-items:center;gap:4px;padding:6px 10px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:13px;color:#4b5054;cursor:pointer;font-family:inherit"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M1 12s4-8 11-8 11 8 11 8-4 8-11 8-11-8-11-8z"/><circle cx="12" cy="12" r="3"/></svg>View</button><button style="display:flex;align-items:center;gap:4px;padding:6px 10px;border:1px solid #e5e5e5;border-radius:8px;background:#fff;font-size:13px;color:#4b5054;cursor:pointer;font-family:inherit"><svg width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg></button></div></td>
                            </tr>
                        </tbody>
                    </table>
                    <div style="display:flex;align-items:center;justify-content:space-between;padding:16px 30px">
                        <span style="font-size:14px;color:#000">Showing 1&ndash;5 of 47</span>
                        <div style="display:flex;gap:4px">
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">&lt;</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#228b22;font-size:14px;font-weight:600;color:#fff;cursor:pointer">1</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">2</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">3</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">...</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">5</button>
                            <button style="width:24px;height:24px;display:flex;align-items:center;justify-content:center;border:1px solid #e5e5e5;border-radius:4px;background:#fff;font-size:14px;font-weight:600;color:#000;cursor:pointer">&gt;</button>
                        </div>
                    </div>
                </div>
            </div>

            <div id="mr-tab-new-brief" class="mr-tab-panel">
                <div style="display:flex;align-items:flex-start;justify-content:space-between;padding:24px 38px 0">
                    <div style="display:flex;flex-direction:column;gap:6px">
                        <div style="display:flex;align-items:center;gap:12px">
                            <div id="mr-new-brief-back" style="cursor:pointer;display:flex">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 12H5"/><polyline points="12 19 5 12 12 5"/></svg>
                            </div>
                            <h1 style="font-size:24px;font-weight:600;color:#000">New Research Brief</h1>
                        </div>
                        <p style="font-size:16px;color:#000">Create a comprehensive research brief for investment analysis</p>
                    </div>
                    <div style="display:flex;gap:12px;align-items:center">
                        <button id="mr-save-draft-btn" style="display:flex;align-items:center;gap:10px;background:none;border:none;padding:10px 12px;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 21H5a2 2 0 0 1-2-2V5a2 2 0 0 1 2-2h11l5 5v11a2 2 0 0 1-2 2z"/><polyline points="17 21 17 13 7 13 7 21"/><polyline points="7 3 7 8 15 8"/></svg>
                            Save Draft
                        </button>
                        <button id="mr-submit-review-btn" style="display:flex;align-items:center;gap:10px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:10px 20px;font-family:inherit;font-size:14px;cursor:pointer">
                            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                            Submit for Review
                        </button>
                    </div>
                </div>
                <div style="display:flex;gap:24px;padding:20px 38px 40px;align-items:flex-start">
                    <div style="background:#fff;border-radius:12px;flex:1;padding:24px 30px 30px;min-width:0">
                        <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:12px">Basic Information</h2>
                        <hr style="border:none;border-top:1px solid #e5e5e5;margin:0 0 16px" />
                        <div style="margin-bottom:20px">
                            <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Research Title *</label>
                            <input type="text" placeholder="Enter a descirptive title for your research brief" style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#4b5054;outline:none;box-sizing:border-box" />
                        </div>
                        <div style="display:flex;gap:20px;margin-bottom:16px">
                            <div style="flex:1">
                                <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Sector/theme*</label>
                                <select style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#000;outline:none;appearance:none;background:#fff  no-repeat right 10px center;background-size:20px;cursor:pointer">
                                    <option>Select Sector</option>
                                </select>
                            </div>
                            <div style="flex:1">
                                <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Investment Type*</label>
                                <select style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#000;outline:none;appearance:none;background:#fff  no-repeat right 10px center;background-size:20px;cursor:pointer">
                                    <option>Select Type</option>
                                </select>
                            </div>
                        </div>
                        <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:12px">Opportunity Description</h2>
                        <hr style="border:none;border-top:1px solid #e5e5e5;margin:0 0 16px" />
                        <div style="margin-bottom:20px">
                            <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Investment Opportunity *</label>
                            <textarea placeholder="Describe the opportunity..." style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#4b5054;outline:none;resize:vertical;min-height:120px;box-sizing:border-box"></textarea>
                            <div style="font-size:14px;color:#4b5054;margin-top:4px">0/2000 Characters</div>
                        </div>
                        <div style="margin-bottom:20px">
                            <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Data Sources &amp; References *</label>
                            <textarea placeholder="List all the data sources or references..." style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#4b5054;outline:none;resize:vertical;min-height:120px;box-sizing:border-box"></textarea>
                        </div>
                        <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:12px">Financial Analysis</h2>
                        <hr style="border:none;border-top:1px solid #e5e5e5;margin:0 0 16px" />
                        <div style="margin-bottom:20px">
                            <div style="font-size:16px;color:#000;margin-bottom:8px">Financial Viability Score: 75%</div>
                            <div style="width:100%;height:10px;background:#d9d9d9;border-radius:12px;position:relative;margin:12px 0 4px">
                                <div style="height:10px;background:#228b22;border-radius:12px;width:73%"></div>
                                <div style="width:18px;height:18px;background:#313eb2;border-radius:50%;position:absolute;top:-4px;left:73%;transform:translateX(-50%);cursor:pointer"></div>
                            </div>
                            <div style="display:flex;justify-content:space-between">
                                <span style="font-size:12px;color:#4b5054">Low Viability</span>
                                <span style="font-size:12px;color:#4b5054">High Viability</span>
                            </div>
                        </div>
                        <div style="margin-bottom:20px">
                            <label style="font-size:16px;color:#000;margin-bottom:8px;display:block">Macroeconomic Impact Assessment</label>
                            <textarea placeholder="Analyze the macroeconomic factors, market trends and potential impact..." style="width:100%;border:1px solid #e5e5e5;border-radius:4px;padding:12px 10px;font-family:inherit;font-size:16px;color:#4b5054;outline:none;resize:vertical;min-height:120px;box-sizing:border-box"></textarea>
                        </div>
                        <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:12px">Supporting Documents</h2>
                        <hr style="border:none;border-top:1px solid #e5e5e5;margin:0 0 16px" />
                        <div style="border:1px solid #228b22;border-radius:12px;padding:40px;display:flex;flex-direction:column;align-items:center;justify-content:center;min-height:203px;cursor:pointer;transition:background 0.2s">
                            <svg width="60" height="60" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M12 16V4"/><polyline points="8 8 12 4 16 8"/><path d="M20 16.7V21a1 1 0 0 1-1 1H5a1 1 0 0 1-1-1v-4.3"/><path d="M4 14a8 8 0 0 1 16 0"/></svg>
                            <div style="font-size:16px;font-weight:600;color:#000">Drag &amp; drop files or browse</div>
                            <div style="font-size:14px;color:#000;margin-top:4px">PDF, XLSX, DOCX, CSV &middot; Max 25MB per file</div>
                        </div>
                    </div>
                    <aside style="width:429px;flex-shrink:0;display:flex;flex-direction:column;gap:20px">
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h3 style="font-size:24px;font-weight:600;color:#000;margin-bottom:16px">Submission Info</h3>
                            <div style="margin-bottom:16px">
                                <div style="font-size:14px;color:#000;margin-bottom:4px">Status</div>
                                <div style="font-size:16px;font-weight:600;color:#000">Draft</div>
                            </div>
                            <div style="margin-bottom:16px">
                                <div style="font-size:14px;color:#000;margin-bottom:4px">Created by</div>
                                <div style="font-size:16px;font-weight:600;color:#000">Research Analyst</div>
                            </div>
                            <div style="margin-bottom:16px">
                                <div style="font-size:14px;color:#000;margin-bottom:4px">Last Modified</div>
                                <div style="font-size:16px;font-weight:600;color:#000">Just now</div>
                            </div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h3 style="font-size:24px;font-weight:600;color:#000;margin-bottom:16px">Shari&rsquo;ah Compliance</h3>
                            <div style="display:flex;align-items:center;gap:10px;background:#228b22;border-radius:12px;padding:12px 20px;margin-bottom:12px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                                <span style="font-size:20px;font-weight:600;color:#000">Compliant</span>
                            </div>
                            <p style="font-size:14px;color:#000;line-height:1.4">This research brief meets Shari&rsquo;ah compliance requirements based on sector and theme selection.</p>
                        </div>
                    </aside>
                </div>
            </div>

            <div id="mr-tab-brief-detail" class="mr-tab-panel">
                <div style="display:flex;align-items:flex-start;justify-content:space-between;padding:24px 38px 0">
                    <div style="display:flex;flex-direction:column;gap:8px">
                        <div style="display:flex;align-items:center;gap:12px">
                            <div id="mr-brief-detail-back" style="cursor:pointer;display:flex">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 12H5"/><polyline points="12 19 5 12 12 5"/></svg>
                            </div>
                            <h1 style="font-size:24px;font-weight:600;color:#000">Green Energy Investment Opportunities in MENA Region</h1>
                        </div>
                        <div style="display:flex;gap:6px;flex-wrap:wrap">
                            <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:12px;font-size:16px;background:#228b22;color:#228b22;">energy</span>
                            <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:12px;font-size:16px;background:#7cfc00;color:#228b22;">Sustainable Development</span>
                            <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:12px;font-size:16px;background:#ff8d28;color:#ff8d28;">Under Review</span>
                            <span style="display:inline-flex;align-items:center;padding:4px 10px;border-radius:12px;font-size:16px;background:#7cfc00;color:#228b22;">Compliant</span>
                        </div>
                    </div>
                    <div style="display:flex;gap:12px;align-items:center">
                        <button style="display:flex;align-items:center;gap:8px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:9px 14px;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                            Export PDF
                        </button>
                        <button style="display:flex;align-items:center;gap:8px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:9px 14px;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M11 4H4a2 2 0 0 0-2 2v14a2 2 0 0 0 2 2h14a2 2 0 0 0 2-2v-7"/><path d="M18.5 2.5a2.121 2.121 0 0 1 3 3L12 15l-4 1 1-4 9.5-9.5z"/></svg>
                            Edit
                        </button>
                        <button style="display:flex;align-items:center;gap:8px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:10px 16px;font-family:inherit;font-size:14px;cursor:pointer">
                            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="20 6 9 17 4 12"/></svg>
                            Approve
                        </button>
                    </div>
                </div>
                <div style="display:flex;gap:24px;padding:20px 38px 40px;align-items:flex-start">
                    <div style="flex:1;display:flex;flex-direction:column;gap:18px;min-width:0">
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:16px">Key Metrics</h2>
                            <div style="display:flex;gap:30px;align-items:flex-end">
                                <div style="display:flex;flex-direction:column;gap:4px">
                                    <span style="font-size:14px;color:#4b5054">Alignment Score</span>
                                    <div style="display:flex;align-items:center;gap:10px">
                                        <div style="width:154px;height:13px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:13px;border-radius:12px;width:90%;background:#228b22"></div></div>
                                        <span style="font-size:24px;font-weight:600;color:#228b22">96</span>
                                    </div>
                                </div>
                                <div style="display:flex;flex-direction:column;gap:4px">
                                    <span style="font-size:14px;color:#4b5054">Viability Score</span>
                                    <div style="display:flex;align-items:center;gap:10px">
                                        <div style="width:154px;height:13px;background:#d9d9d9;border-radius:12px;overflow:hidden"><div style="height:13px;border-radius:12px;width:71%;background:#7cfc00"></div></div>
                                        <span style="font-size:24px;font-weight:600;color:#228b22">84</span>
                                    </div>
                                </div>
                                <div style="display:flex;flex-direction:column;gap:4px">
                                    <span style="font-size:14px;color:#4b5054">Completion Date</span>
                                    <span style="font-size:24px;font-weight:600;color:#0f151f">2024-02-01</span>
                                </div>
                            </div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:16px">Investment Opportunity</h2>
                            <p style="font-size:16px;color:#000;line-height:1.6">The MENA region presents significant opportunities for green energy investments, particularly in solar and wind power infrastructure. With abundant natural resources and increasing government support for renewable energy initiatives, the market shows strong potential for sustainable growth. Key drivers include: 1) Government commitments to reduce carbon emissions by 40% by 2030, 2) Declining costs of renewable energy technology, 3) Growing demand for clean energy solutions, 4) Strategic geographic positioning for solar energy generation. The investment opportunity focuses on developing utility-scale solar farms and wind energy projects across Saudi Arabia, UAE, and Egypt, with projected IRR of 12-15% over a 20-year period.</p>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:16px">
                                <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:0">Sector Growth Trends</h2>
                                <button style="display:flex;align-items:center;gap:8px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:9px 14px;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">Last 6 Months <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><polyline points="6 9 12 15 18 9"/></svg></button>
                            </div>
                            <div style="position:relative;height:260px">
                                <div style="position:absolute;left:72px;bottom:40px;width:70px;height:143px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:72px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">Jan</div>
                                <div style="position:absolute;left:72px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">65%</div>
                                <div style="position:absolute;left:184px;bottom:40px;width:70px;height:169px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:184px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">Feb</div>
                                <div style="position:absolute;left:184px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">72%</div>
                                <div style="position:absolute;left:296px;bottom:40px;width:70px;height:106px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:296px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">Mar</div>
                                <div style="position:absolute;left:296px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">55%</div>
                                <div style="position:absolute;left:408px;bottom:40px;width:70px;height:143px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:408px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">Apr</div>
                                <div style="position:absolute;left:408px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">66%</div>
                                <div style="position:absolute;left:520px;bottom:40px;width:70px;height:181px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:520px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">May</div>
                                <div style="position:absolute;left:520px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">75%</div>
                                <div style="position:absolute;left:632px;bottom:40px;width:70px;height:204px;background:#228b22;border-radius:4px 4px 0 0;"></div>
                                <div style="position:absolute;left:632px;bottom:14px;width:70px;text-align:center;font-size:14px;color:#4b5054;">Jun</div>
                                <div style="position:absolute;left:632px;bottom:-8px;width:70px;text-align:center;font-size:16px;font-weight:600;color:#000;">85%</div>
                            </div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:16px">Macroeconomic Impact Assessment</h2>
                            <p style="font-size:16px;color:#000;line-height:1.6">The macroeconomic environment strongly supports renewable energy investments in the MENA region. Oil-dependent economies are actively diversifying their energy portfolios, creating favorable policy frameworks and financial incentives. Regional GDP growth averaging 3.5% annually, coupled with population growth of 2.1%, drives increasing energy demand. Government initiatives like Saudi Vision 2030 and UAE Energy Strategy 2050 provide long-term policy stability. Currency stability in GCC countries reduces forex risk, while sovereign wealth fund participation signals strong institutional support.</p>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:16px">Data Sources &amp; References</h2>
                            <p style="font-size:16px;color:#000;line-height:1.6">1. International Energy Agency (IEA) - MENA Energy Outlook 2023<br />2. World Bank - Renewable Energy Market Analysis<br />3. IRENA - Renewable Energy Statistics 2023<br />4. Bloomberg New Energy Finance - MENA Solar Report<br />5. Regional government energy strategy documents<br />6. Industry expert interviews and market surveys</p>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px;border:1px solid #e5e5e5">
                            <h2 style="font-size:20px;font-weight:600;color:#000;margin-bottom:16px">Comments &amp; Feedback</h2>
                            <div style="background:#e5e5e5;border-radius:12px;padding:12px 20px;margin-bottom:12px">
                                <div style="display:flex;justify-content:space-between"><div><div style="font-size:16px;">Dr. Hassan Adamu</div><div style="font-size:14px;color:#4b5054;">Senior Supervisor</div></div><div style="font-size:14px;color:#4b5054;">2024-04-16</div></div>
                                <p style="font-size:14px;color:#4b5054;margin-top:8px;line-height:1.5;">Excellent research brief. The financial projections are well-supported by market data. Please add more detail on regulatory compliance requirements.</p>
                            </div>
                            <div style="background:#e5e5e5;border-radius:12px;padding:12px 20px;margin-bottom:12px">
                                <div style="display:flex;justify-content:space-between"><div><div style="font-size:16px;">Dr. Hassan Adamu</div><div style="font-size:14px;color:#4b5054;">Senior Supervisor</div></div><div style="font-size:14px;color:#4b5054;">2024-04-16</div></div>
                                <p style="font-size:14px;color:#4b5054;margin-top:8px;line-height:1.5;">Excellent research brief. The financial projections are well-supported by market data. Please add more detail on regulatory compliance requirements.</p>
                            </div>
                            <div style="background:#fff;border:1px solid #e5e5e5;border-radius:12px;padding:12px 20px;margin-bottom:12px"><span style="font-size:14px;color:#c4c4c4;">Add your comment or feedback</span></div>
                            <button style="display:flex;align-items:center;gap:8px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:10px 16px;font-family:inherit;font-size:16px;cursor:pointer">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><line x1="22" y1="2" x2="11" y2="13"/><polygon points="22 2 15 22 11 13 2 9 22 2"/></svg>
                                Post Comment
                            </button>
                        </div>
                    </div>
                    <div style="width:429px;flex-shrink:0;display:flex;flex-direction:column;gap:18px">
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h3 style="font-size:24px;font-weight:600;color:#000;margin-bottom:16px">Research Information</h3>
                            <div style="margin-bottom:16px"><div style="font-size:14px;color:#4b5054;">Research ID</div><div style="font-size:16px;font-weight:600;">RB-0001</div></div>
                            <div style="margin-bottom:16px"><div style="font-size:14px;color:#4b5054;">Lead Analyst</div><div style="font-size:16px;font-weight:600;">Sarah Ahmed</div></div>
                            <div style="margin-bottom:16px"><div style="font-size:14px;color:#4b5054;">Submitted Date</div><div style="font-size:16px;font-weight:600;">2024-02-01</div></div>
                            <div><div style="font-size:14px;color:#4b5054;">Current Status</div><div style="margin-top:4px"><span style="display:inline-flex;padding:4px 10px;border-radius:12px;font-size:16px;background:#eff31c;font-size:16px;">Under review</span></div></div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h3 style="font-size:24px;font-weight:600;color:#000;margin-bottom:16px">Approval Workflow</h3>
                            <div style="display:flex;align-items:flex-start;gap:12px;margin-bottom:16px">
                                <div style="width:31px;height:31px;border-radius:50%;background:#228b22;display:flex;align-items:center;justify-content:center;font-size:14px;color:#fff;flex-shrink:0;">&#10003;</div>
                                <div><div style="font-size:16px;font-weight:600;">Submitted</div><div style="font-size:14px;color:#000;">Sarah Ahmed<br />2024-02-01</div></div>
                            </div>
                            <div style="display:flex;align-items:flex-start;gap:12px;margin-bottom:16px">
                                <div style="width:31px;height:31px;border-radius:50%;background:#eff31c;display:flex;align-items:center;justify-content:center;font-size:14px;color:#fff;flex-shrink:0;">&#10003;</div>
                                <div><div style="font-size:16px;font-weight:600;">Under Review</div><div style="font-size:14px;color:#000;">Sarah Ahmed<br />2024-02-01</div></div>
                            </div>
                            <div style="display:flex;align-items:flex-start;gap:12px;margin-bottom:16px">
                                <div style="width:31px;height:31px;border-radius:50%;background:#c4c4c4;display:flex;align-items:center;justify-content:center;font-size:14px;color:#666;flex-shrink:0;">&#8226;&#8226;&#8226;</div>
                                <div><div style="font-size:16px;font-weight:600;">Risk Assessment</div></div>
                            </div>
                            <div style="display:flex;align-items:flex-start;gap:12px;margin-bottom:16px">
                                <div style="width:31px;height:31px;border-radius:50%;background:#c4c4c4;display:flex;align-items:center;justify-content:center;font-size:14px;color:#666;flex-shrink:0;">&#8226;&#8226;&#8226;</div>
                                <div><div style="font-size:16px;font-weight:600;">Approved</div></div>
                            </div>
                        </div>
                        <div style="background:#fff;border-radius:12px;padding:24px 30px">
                            <h3 style="font-size:24px;font-weight:600;color:#000;margin-bottom:16px">Supporting Documents</h3>
                            <div style="display:flex;align-items:center;gap:12px;background:#d9d9d9;border-radius:8px;padding:14px 16px;margin-bottom:10px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                <div style="flex:1"><div style="font-size:16px;font-weight:600;">Market Analysis Report.pdf</div><div style="font-size:14px;color:#000;">2.4 MB</div></div>
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                            </div>
                            <div style="display:flex;align-items:center;gap:12px;background:#d9d9d9;border-radius:8px;padding:14px 16px;margin-bottom:10px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                <div style="flex:1"><div style="font-size:16px;font-weight:600;">Market Analysis Report.pdf</div><div style="font-size:14px;color:#000;">2.4 MB</div></div>
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                            </div>
                            <div style="display:flex;align-items:center;gap:12px;background:#d9d9d9;border-radius:8px;padding:14px 16px;margin-bottom:10px">
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="#e50303" stroke-width="2" style="flex-shrink:0"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6"/></svg>
                                <div style="flex:1"><div style="font-size:16px;font-weight:600;">Market Analysis Report.pdf</div><div style="font-size:14px;color:#000;">2.4 MB</div></div>
                                <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" style="cursor:pointer"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="7 10 12 15 17 10"/><line x1="12" y1="15" x2="12" y2="3"/></svg>
                            </div>
                        </div>
                    </div>
                </div>
            </div>

            <div id="mr-tab-approval-flow" class="mr-tab-panel">
                <div style="display:flex;align-items:flex-start;justify-content:space-between;padding:24px 38px 0">
                    <div style="display:flex;flex-direction:column;gap:6px">
                        <div style="display:flex;align-items:center;gap:12px">
                            <div id="mr-approval-flow-back" style="cursor:pointer;display:flex">
                                <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M19 12H5"/><polyline points="12 19 5 12 12 5"/></svg>
                            </div>
                            <h1 style="font-size:24px;font-weight:600;color:#000">Approval Workflow Queue</h1>
                        </div>
                        <p style="font-size:16px;color:#000">3 briefs pending your action &middot; Supervisor view</p>
                    </div>
                    <div style="display:flex;gap:12px;align-items:center">
                        <button style="display:flex;align-items:center;gap:10px;background:#fff;border:1px solid #e5e5e5;border-radius:8px;padding:9px 16px;font-family:inherit;font-size:14px;color:#4b5054;cursor:pointer">
                            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 15v4a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2v-4"/><polyline points="17 8 12 3 7 8"/><line x1="12" y1="3" x2="12" y2="15"/></svg>
                            Export
                        </button>
                        <button style="display:flex;align-items:center;gap:10px;background:#228b22;color:#fff;border:none;border-radius:8px;padding:9px 16px;font-family:inherit;font-size:14px;cursor:pointer">
                            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01"/></svg>
                            Bulk Approve
                        </button>
                    </div>
                </div>
                <div style="display:flex;flex-direction:column;gap:24px;padding:20px 38px 40px">
                    <div style="background:#fff;border-radius:12px;overflow:hidden">
                        <div style="display:flex;align-items:center;gap:12px;padding:20px 20px 0;flex-wrap:wrap">
                            <div style="width:39px;height:39px;flex-shrink:0;display:flex;align-items:center;justify-content:center">
                                <svg width="39" height="39" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M18 20V10"/><path d="M12 20V4"/><path d="M6 20v-6"/></svg>
                            </div>
                            <div>
                                <div style="font-size:16px;font-weight:600;color:#000">Sukuk Market Dynamics &mdash; H1 2026 Outlook</div>
                                <div style="display:flex;gap:8px;align-items:center;margin-top:4px">
                                    <span style="font-size:14px;font-weight:600;color:#000">By Omar Suleiman &middot; Submitted Feb 22, 2026</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#eff31c;color:#ac7f5e">IN REVIEW</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#228b22;color:#fff">0 COMPLIANT</span>
                                </div>
                            </div>
                            <div style="margin-left:auto;display:flex;gap:8px">
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#4b5054">View Brief</button>
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#4b5054">Request Changes</button>
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;background:#228b22;color:#fff;border:1px solid #228b22">Approve</button>
                            </div>
                        </div>
                        <div style="display:flex;gap:0;padding:16px 20px 20px;border-top:1px solid #e5e5e5;margin-top:16px">
                            <div style="flex:1"><div style="font-size:14px;color:#000;margin-bottom:4px">Alignment Score</div><div style="font-size:24px;font-weight:600;color:#000">88</div></div>
                            <div style="flex:1"><div style="font-size:14px;color:#000;margin-bottom:4px">Viability Score</div><div style="font-size:24px;font-weight:600;color:#000">83</div></div>
                            <div style="flex:1"><div style="font-size:14px;color:#000;margin-bottom:4px">Risk Level</div><div style="font-size:24px;font-weight:600;color:#000">Medium</div></div>
                            <div style="flex:1"><div style="font-size:14px;color:#000;margin-bottom:4px">Days in Queue</div><div style="font-size:24px;font-weight:600;color:#000">4d</div></div>
                        </div>
                    </div>
                    <div style="background:#fff;border-radius:12px;overflow:hidden">
                        <div style="display:flex;align-items:center;gap:16px;padding:16px 20px;background:#e50303">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="flex-shrink:0;color:#e50303"><path d="M1 21h22L12 2 1 21zm12-3h-2v-2h2v2zm0-4h-2v-4h2v4z"/></svg>
                            <span style="font-size:14px;color:#fff">Compliance concern flagged by Shari&rsquo;ah board &mdash; requires revision</span>
                        </div>
                        <div style="display:flex;align-items:center;gap:12px;padding:20px 20px 0;flex-wrap:wrap">
                            <div style="width:39px;height:39px;flex-shrink:0;display:flex;align-items:center;justify-content:center">
                                <svg width="39" height="39" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M18 20V10"/><path d="M12 20V4"/><path d="M6 20v-6"/></svg>
                            </div>
                            <div>
                                <div style="font-size:16px;font-weight:600;color:#000">Sukuk Market Dynamics &mdash; H1 2026 Outlook</div>
                                <div style="display:flex;gap:8px;align-items:center;margin-top:4px">
                                    <span style="font-size:14px;font-weight:600;color:#000">By Omar Suleiman &middot; Submitted Feb 22, 2026</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#eff31c;color:#ac7f5e">FLAGGED</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#eff31c;color:#ac7f5e">PENDING SHARI&rsquo;AH REVIEW</span>
                                </div>
                            </div>
                            <div style="margin-left:auto;display:flex;gap:8px">
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#4b5054">View</button>
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;background:#e50303;color:#fff;border:1px solid #e50303">Return for Revision</button>
                            </div>
                        </div>
                    </div>
                    <div style="background:#fff;border-radius:12px;overflow:hidden">
                        <div style="display:flex;align-items:center;gap:16px;padding:16px 20px;background:#228b22">
                            <svg width="24" height="24" viewBox="0 0 24 24" fill="currentColor" style="flex-shrink:0;color:#228b22"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"/><polyline points="22 4 12 14.01 9 11.01" fill="none" stroke="currentColor" stroke-width="2"/></svg>
                            <span style="font-size:14px;color:#fff">Compliance concern flagged by Shari&rsquo;ah board &mdash; requires revision</span>
                        </div>
                        <div style="display:flex;align-items:center;gap:12px;padding:20px 20px 0;flex-wrap:wrap">
                            <div style="width:39px;height:39px;flex-shrink:0;display:flex;align-items:center;justify-content:center">
                                <svg width="39" height="39" viewBox="0 0 24 24" fill="none" stroke="#228b22" stroke-width="2"><path d="M18 20V10"/><path d="M12 20V4"/><path d="M6 20v-6"/></svg>
                            </div>
                            <div>
                                <div style="font-size:16px;font-weight:600;color:#000">Sukuk Market Dynamics &mdash; H1 2026 Outlook</div>
                                <div style="display:flex;gap:8px;align-items:center;margin-top:4px">
                                    <span style="font-size:14px;font-weight:600;color:#000">By Omar Suleiman &middot; Submitted Feb 22, 2026</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#cb30e0;color:#fff">READY</span>
                                    <span style="display:inline-flex;align-items:center;padding:3px 10px;border-radius:8px;font-size:14px;background:#228b22;color:#fff">COMPLIANT</span>
                                </div>
                            </div>
                            <div style="margin-left:auto;display:flex;gap:8px">
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#4b5054">View Brief</button>
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;border:1px solid #e5e5e5;background:#fff;color:#4b5054">Request Changes</button>
                                <button style="display:inline-flex;align-items:center;padding:8px 12px;border-radius:8px;font-family:inherit;font-size:14px;cursor:pointer;background:#228b22;color:#fff;border:1px solid #228b22">Approve</button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>


</div>
</template>
<script setup>
import { ref } from "vue";
</script>