import React, { useState } from 'react';
import { Share2, Plus, X } from 'lucide-react';

const TotalCompCalculator = () => {
  const [baseSalary, setBaseSalary] = useState('75000');
  const [companyName, setCompanyName] = useState('');
  const [jobTitle, setJobTitle] = useState('');
  const [perks, setPerks] = useState([
    { name: '401k Match', value: '3750', id: 1 },
    { name: 'Health Insurance', value: '8400', id: 2 },
    { name: 'Annual Bonus', value: '7500', id: 3 }
  ]);
  const [newPerk, setNewPerk] = useState({ name: '', value: '' });
  const [showReceipt, setShowReceipt] = useState(false);

  const quickPerks = [
    '401k Match', 'Health Insurance', 'Stock/RSUs', 'Annual Bonus',
    'PTO Value', 'Gym/Wellness', 'Free Food', 'Commuter',
    'Education', 'Phone/Internet', 'WFH Stipend', 'Equity'
  ];

  const totalPerks = perks.reduce((sum, perk) => sum + (parseFloat(perk.value) || 0), 0);
  const salary = parseFloat(baseSalary) || 0;
  const totalComp = salary + totalPerks;
  const percentIncrease = salary > 0 ? ((totalPerks / salary) * 100).toFixed(1) : 0;

  const addQuickPerk = (name) => {
    setPerks([...perks, { name, value: '', id: Date.now() }]);
  };

  const addCustomPerk = () => {
    if (newPerk.name) {
      setPerks([...perks, { ...newPerk, id: Date.now() }]);
      setNewPerk({ name: '', value: '' });
    }
  };

  const removePerk = (id) => {
    setPerks(perks.filter(p => p.id !== id));
  };

  const updatePerk = (id, field, value) => {
    setPerks(perks.map(p => p.id === id ? { ...p, [field]: value } : p));
  };

  const handleShare = () => {
    const text = `💰 MY TOTAL COMP RECEIPT 💰\n\nBase Salary: $${salary.toLocaleString()}\nPerks & Benefits: $${totalPerks.toLocaleString()}\n${'─'.repeat(25)}\nTOTAL: $${totalComp.toLocaleString()}\n\nThat's ${percentIncrease}% more than my base!\n\nGet your receipt:`;
    
    if (navigator.share) {
      navigator.share({ text });
    } else {
      navigator.clipboard.writeText(text);
      alert('Copied to clipboard!');
    }
  };

  const calculateDate = () => {
    const date = new Date();
    return date.toLocaleDateString('en-US', { month: '2-digit', day: '2-digit', year: 'numeric' });
  };

  return (
    <div className="min-h-screen bg-zinc-900 p-4 flex items-center justify-center">
      <div className="w-full max-w-md">
        
        {!showReceipt ? (
          <div className="bg-white p-8 shadow-2xl">
            <div className="border-b-2 border-dashed border-gray-300 pb-6 mb-6">
              <div className="text-center mb-2">
                <div className="text-xs tracking-widest text-gray-500 mb-1">TOTAL COMPENSATION</div>
                <div className="text-2xl font-bold tracking-tight">CALCULATOR</div>
              </div>
            </div>

            <div className="space-y-6 font-mono text-sm">
              <div>
                <div className="text-gray-400 text-xs tracking-wide mb-2">OPTIONAL</div>
                <input
                  type="text"
                  value={companyName}
                  onChange={(e) => setCompanyName(e.target.value)}
                  placeholder="Company Name"
                  className="w-full px-2 py-2 border border-gray-200 outline-none focus:border-gray-400 mb-2 text-xs tracking-wide"
                />
                <input
                  type="text"
                  value={jobTitle}
                  onChange={(e) => setJobTitle(e.target.value)}
                  placeholder="Job Title"
                  className="w-full px-2 py-2 border border-gray-200 outline-none focus:border-gray-400 text-xs tracking-wide"
                />
              </div>

              <div>
                <div className="flex justify-between items-baseline mb-2">
                  <span className="text-gray-600 tracking-wide">BASE SALARY</span>
                  <span className="text-xs text-gray-400">ANNUAL</span>
                </div>
                <div className="flex items-baseline border-b-2 border-black pb-1">
                  <span className="text-lg mr-1">$</span>
                  <input
                    type="number"
                    value={baseSalary}
                    onChange={(e) => setBaseSalary(e.target.value)}
                    placeholder="0"
                    className="flex-1 text-xl outline-none"
                  />
                </div>
              </div>

              <div>
                <div className="text-gray-600 tracking-wide mb-3">PERKS & BENEFITS</div>
                
                <div className="flex flex-wrap gap-2 mb-4">
                  {quickPerks.map((name, idx) => (
                    <button
                      key={idx}
                      onClick={() => addQuickPerk(name)}
                      className="px-2 py-1 text-xs bg-gray-100 hover:bg-gray-200 border border-gray-300 transition"
                    >
                      + {name}
                    </button>
                  ))}
                </div>

                {perks.length > 0 && (
                  <div className="space-y-3 mb-4">
                    {perks.map((perk) => (
                      <div key={perk.id} className="flex items-start gap-2 text-xs">
                        <div className="flex-1">
                          <input
                            type="text"
                            value={perk.name}
                            onChange={(e) => updatePerk(perk.id, 'name', e.target.value)}
                            className="w-full mb-1 px-2 py-1 border border-gray-300 outline-none focus:border-black uppercase tracking-wide"
                            placeholder="PERK NAME"
                          />
                          <div className="flex items-baseline border-b border-black pb-1">
                            <span className="mr-1">$</span>
                            <input
                              type="number"
                              value={perk.value}
                              onChange={(e) => updatePerk(perk.id, 'value', e.target.value)}
                              placeholder="0"
                              className="flex-1 outline-none"
                            />
                          </div>
                        </div>
                        <button
                          onClick={() => removePerk(perk.id)}
                          className="p-1 hover:bg-gray-200 transition"
                        >
                          <X size={14} />
                        </button>
                      </div>
                    ))}
                  </div>
                )}

                <div className="flex gap-2 text-xs">
                  <input
                    type="text"
                    value={newPerk.name}
                    onChange={(e) => setNewPerk({ ...newPerk, name: e.target.value })}
                    placeholder="Custom perk name"
                    className="flex-1 px-2 py-2 border border-gray-300 outline-none focus:border-black"
                  />
                  <button
                    onClick={addCustomPerk}
                    className="px-4 py-2 bg-black text-white hover:bg-gray-800 transition"
                  >
                    <Plus size={14} />
                  </button>
                </div>
              </div>
            </div>

            <button
              onClick={() => setShowReceipt(true)}
              className="w-full mt-8 py-4 bg-black text-white font-mono text-sm tracking-widest hover:bg-gray-800 transition"
            >
              GENERATE RECEIPT
            </button>
            
            <div className="text-center mt-4 text-xs text-gray-400">
              Pre-filled with example values - edit to match yours
            </div>
          </div>
        ) : (
          <div className="bg-white shadow-2xl">
            {/* Receipt Header */}
            <div className="bg-black text-white p-6 text-center">
              <div className="text-xs tracking-widest mb-2">YOUR TOTAL COMP</div>
              <div className="text-3xl font-bold font-mono">RECEIPT</div>
            </div>

            <div className="p-8 font-mono text-sm">
              {(companyName || jobTitle) && (
                <div className="mb-6 pb-4 border-b border-gray-200">
                  {companyName && <div className="text-xs tracking-widest mb-1">{companyName.toUpperCase()}</div>}
                  {jobTitle && <div className="text-xs text-gray-600">{jobTitle}</div>}
                </div>
              )}

              <div className="flex justify-between text-xs mb-6 pb-4 border-b border-dashed border-gray-300">
                <span>DATE: {calculateDate()}</span>
                <span>TIME: {new Date().toLocaleTimeString('en-US', { hour: '2-digit', minute: '2-digit' })}</span>
              </div>

              {/* Items */}
              <div className="space-y-2 mb-4">
                <div className="flex justify-between">
                  <span className="tracking-wide">BASE SALARY</span>
                  <span className="font-bold">${salary.toLocaleString()}</span>
                </div>
                
                {perks.length > 0 && (
                  <div className="ml-4 space-y-2 my-3">
                    {perks.map((perk) => (
                      <div key={perk.id} className="flex justify-between text-xs">
                        <span className="text-gray-600 uppercase">{perk.name}</span>
                        <span className="text-gray-600">${parseFloat(perk.value || 0).toLocaleString()}</span>
                      </div>
                    ))}
                  </div>
                )}

                <div className="flex justify-between pt-2 border-t border-dashed border-gray-300">
                  <span className="tracking-wide">PERKS SUBTOTAL</span>
                  <span className="font-bold">${totalPerks.toLocaleString()}</span>
                </div>
              </div>

              {/* Total */}
              <div className="border-t-4 border-double border-black pt-4 mb-6">
                <div className="flex justify-between items-baseline">
                  <span className="text-lg tracking-widest">TOTAL</span>
                  <span className="text-3xl font-bold">${totalComp.toLocaleString()}</span>
                </div>
                <div className="text-right text-xs text-gray-500 mt-1">per year</div>
              </div>

              {/* Stats Box */}
              <div className="bg-black text-white p-4 mb-6 text-center">
                <div className="text-xs tracking-widest mb-1">YOU'RE EARNING</div>
                <div className="text-4xl font-bold mb-1">{percentIncrease}%</div>
                <div className="text-xs tracking-wide">MORE THAN YOUR BASE SALARY</div>
              </div>

              {/* Breakdown Chart */}
              <div className="mb-6">
                <div className="text-xs text-gray-600 mb-2 tracking-wide">BREAKDOWN</div>
                <div className="h-8 flex overflow-hidden border border-gray-300">
                  <div 
                    className="bg-black flex items-center justify-center text-white text-xs"
                    style={{ width: `${(salary/totalComp)*100}%` }}
                  >
                    {((salary/totalComp)*100).toFixed(0)}%
                  </div>
                  <div 
                    className="bg-gray-300 flex items-center justify-center text-black text-xs"
                    style={{ width: `${(totalPerks/totalComp)*100}%` }}
                  >
                    {((totalPerks/totalComp)*100).toFixed(0)}%
                  </div>
                </div>
                <div className="flex justify-between text-xs mt-1 text-gray-600">
                  <span>■ Base</span>
                  <span>■ Perks</span>
                </div>
              </div>

              {/* Buttons */}
              <div className="space-y-2">
                <button
                  onClick={handleShare}
                  className="w-full py-3 bg-black text-white font-mono text-xs tracking-widest hover:bg-gray-800 transition flex items-center justify-center gap-2"
                >
                  <Share2 size={14} />
                  SHARE RECEIPT
                </button>
                <button
                  onClick={() => setShowReceipt(false)}
                  className="w-full py-3 border-2 border-black font-mono text-xs tracking-widest hover:bg-gray-100 transition"
                >
                  RECALCULATE
                </button>
              </div>

              {/* Footer */}
              <div className="mt-6 pt-4 border-t border-dashed border-gray-300 text-center text-xs text-gray-400">
                <div>THANK YOU FOR CALCULATING</div>
                <div className="mt-2">* * * * *</div>
              </div>
            </div>

            {/* Tear line */}
            <div className="border-t-2 border-dashed border-gray-300"></div>
            <div className="h-4"></div>
          </div>
        )}
      </div>
    </div>
  );
};

export default TotalCompCalculator;
