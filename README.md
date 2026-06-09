import React, { useState, useEffect, useRef } from 'react';
import { 
  Heart, 
  Calendar, 
  Plus, 
  TrendingUp, 
  Activity, 
  Settings, 
  MessageSquare, 
  BookOpen, 
  Droplet, 
  Scale, 
  Award, 
  ChevronRight, 
  Sparkles, 
  Trash2, 
  User, 
  ArrowRight,
  CheckCircle,
  AlertCircle,
  FileText,
  Calculator,
  BrainCircuit,
  ClipboardList
} from 'lucide-react';
import { 
  LineChart, 
  Line, 
  BarChart, 
  Bar, 
  XAxis, 
  YAxis, 
  CartesianGrid, 
  Tooltip, 
  Legend, 
  ResponsiveContainer, 
  PieChart, 
  Pie, 
  Cell 
} from 'recharts';

// 預設寵物數據 (已新增你在截圖中展示的 jiu，並保留麻吉與露娜)
const DEFAULT_PETS = [
  {
    id: 'pet-3',
    name: 'jiu',
    type: 'cat',
    breed: '狸花',
    age: '1 歲',
    weight: 4.3,
    status: 'neutered', // 已結紮
    targetCalories: 400, // 截圖所設之目標
    targetWater: 300,    // 截圖所設之目標
    avatar: '🐈',
    birthdate: '2025-06-01',
    personality: '聰明活潑，好奇心旺盛的狸花貓，對流動的水特別感興趣。'
  },
  {
    id: 'pet-1',
    name: '麻吉 (Mochi)',
    type: 'dog',
    breed: '柴犬',
    age: '2 歲 5 個月',
    weight: 9.8,
    status: 'neutered',
    targetCalories: 580,
    targetWater: 588,
    avatar: '🐕',
    birthdate: '2023-12-15',
    personality: '固執但溫柔的柴犬，外出散步時非常有活力。'
  },
  {
    id: 'pet-2',
    name: '露娜 (Luna)',
    type: 'cat',
    breed: '布偶貓',
    age: '1 歲 2 個月',
    weight: 4.2,
    status: 'neutered',
    targetCalories: 246,
    targetWater: 210,
    avatar: '🐈',
    birthdate: '2025-04-01',
    personality: '黏人溫順的小公主，食量比較秀氣。'
  }
];
