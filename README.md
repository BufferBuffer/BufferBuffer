import React from "react";
import { FaFileInvoice, FaExchangeAlt, FaFileAlt, FaReceipt, FaMoneyBill, FaBook, FaUndo, FaRedo, FaMobile, FaBalanceScale, FaChartLine, FaClipboardList, FaFileExcel, FaWhatsapp, FaSms, FaToolbox, FaCog, FaKey, FaUserShield, FaUser, FaPhone, FaPowerOff } from "react-icons/fa";

const TramSoftUI = () => {
  return (
    <div className="bg-gray-900 text-white h-screen overflow-auto flex flex-col items-center py-8 px-4">
      <h1 className="text-3xl font-bold mb-4">TRAM SOFT</h1>
      
      <div className="bg-gray-800 p-2 rounded-lg mb-4 text-center">
        <span className="text-sm">🕒 10:53:24 AM | 📅 19-2-2025</span>
      </div>
      
      <div className="grid grid-cols-4 gap-4 w-full max-w-6xl">
        {/* Daily Books */}
        <div className="bg-white text-black p-4 rounded-lg shadow-lg">
          <h2 className="font-semibold text-lg mb-2">Daily Books</h2>
          {[
            { text: "Purchase Invoices", color: "bg-red-500", icon: <FaFileInvoice /> },
            { text: "Godown Transfer", color: "bg-orange-500", icon: <FaExchangeAlt /> },
            { text: "Invoices", color: "bg-yellow-500", icon: <FaFileAlt /> },
            { text: "Receipts", color: "bg-green-500", icon: <FaReceipt /> },
            { text: "Payments", color: "bg-blue-500", icon: <FaMoneyBill /> },
            { text: "Journal Vouchers", color: "bg-indigo-500", icon: <FaBook /> },
            { text: "Sale Return", color: "bg-pink-500", icon: <FaUndo /> },
            { text: "Purchase Return", color: "bg-rose-500", icon: <FaRedo /> },
            { text: "IMEI Tracking", color: "bg-teal-500", icon: <FaMobile /> },
          ].map((btn, idx) => (
            <button key={idx} className={`w-full text-white py-2 my-1 rounded ${btn.color} flex items-center justify-center`}>
              {btn.icon} <span className="ml-2">{btn.text}</span>
            </button>
          ))}
        </div>
        
        {/* Special Books */}
        <div className="bg-white text-black p-4 rounded-lg shadow-lg">
          <h2 className="font-semibold text-lg mb-2">Special Books</h2>
          {[
            { text: "Assets Ledger", color: "bg-red-500", icon: <FaBalanceScale /> },
            { text: "Liabilities Ledger", color: "bg-orange-500", icon: <FaChartLine /> },
            { text: "Capital Ledger", color: "bg-yellow-500", icon: <FaClipboardList /> },
            { text: "Accounts Manager", color: "bg-green-500", icon: <FaUserShield /> },
            { text: "Expenses Ledger", color: "bg-blue-500", icon: <FaMoneyBill /> },
            { text: "Revenue Ledger", color: "bg-indigo-500", icon: <FaChartLine /> },
            { text: "Stock Ledger", color: "bg-purple-500", icon: <FaClipboardList /> },
            { text: "Stock Manager", color: "bg-pink-500", icon: <FaToolbox /> },
            { text: "Accessories", color: "bg-teal-500", icon: <FaCog /> },
          ].map((btn, idx) => (
            <button key={idx} className={`w-full text-white py-2 my-1 rounded ${btn.color} flex items-center justify-center`}>
              {btn.icon} <span className="ml-2">{btn.text}</span>
            </button>
          ))}
        </div>
        
        {/* Financial Statements */}
        <div className="bg-white text-black p-4 rounded-lg shadow-lg">
          <h2 className="font-semibold text-lg mb-2">Financial Statements</h2>
          {[
            { text: "Trial Balance", color: "bg-red-500", icon: <FaBalanceScale /> },
            { text: "Aged Trial Balance", color: "bg-orange-500", icon: <FaChartLine /> },
            { text: "Income Statement", color: "bg-yellow-500", icon: <FaClipboardList /> },
            { text: "Balance Sheet", color: "bg-green-500", icon: <FaFileExcel /> },
            { text: "Profit & Loss", color: "bg-blue-500", icon: <FaChartLine /> },
            { text: "All Accounts", color: "bg-indigo-500", icon: <FaBook /> },
            { text: "Aging Report", color: "bg-purple-500", icon: <FaClipboardList /> },
            { text: "All Reports", color: "bg-pink-500", icon: <FaFileExcel /> },
            { text: "Excel/Pdf E & I", color: "bg-teal-500", icon: <FaFileExcel /> },
          ].map((btn, idx) => (
            <button key={idx} className={`w-full text-white py-2 my-1 rounded ${btn.color} flex items-center justify-center`}>
              {btn.icon} <span className="ml-2">{btn.text}</span>
            </button>
          ))}
        </div>
        
        {/* Other Options */}
        <div className="bg-white text-black p-4 rounded-lg shadow-lg">
          <h2 className="font-semibold text-lg mb-2">Other Options</h2>
          {[
            { text: "WhatsApp", color: "bg-green-600", icon: <FaWhatsapp /> },
            { text: "SMS", color: "bg-blue-600", icon: <FaSms /> },
            { text: "Utilities", color: "bg-purple-600", icon: <FaToolbox /> },
            { text: "Settings", color: "bg-gray-600", icon: <FaCog /> },
            { text: "License", color: "bg-red-600", icon: <FaKey /> },
            { text: "Activation", color: "bg-orange-600", icon: <FaUserShield /> },
            { text: "Tasawwur Raza Attari", color: "bg-blue-800", icon: <FaUser /> },
            { text: "03123267226", color: "bg-green-800", icon: <FaPhone /> },
            { text: "Exit", color: "bg-red-800", icon: <FaPowerOff /> },
          ].map((btn, idx) => (
            <button key={idx} className={`w-full text-white py-2 my-1 rounded ${btn.color} flex items-center justify-center`}>
              {btn.icon} <span className="ml-2">{btn.text}</span>
            </button>
          ))}
        </div>
      </div>
    </div>
  );
};

export default TramSoftUI;
