"use client";
import React, { useState } from 'react';

export default function BookingPage() {
  const [formData, setFormData] = useState({
    name: '',
    date: '',
    service: 'corrective-exercise'
  });

  const handleSubmit = (e: React.FormEvent) => {
    e.preventDefault();
    alert(`درخواست رزرو برای ${formData.name} ثبت شد! (در مرحله بعد به درگاه وصل می‌شود)`);
    console.log("Submitted Data:", formData);
