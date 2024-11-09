import React from 'react';
import { Phone, Mail, Home } from 'lucide-react';

const DeveloperProfile = () => {
  return (
    <div className="min-h-screen bg-gradient-to-br from-orange-50 to-blue-50 p-8 max-w-4xl mx-auto font-sans">
      <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
        {/* Left Column */}
        <div className="space-y-6">
          {/* Profile Image */}
          <div className="relative">
            <div className="w-full aspect-square rounded-lg overflow-hidden shadow-lg border-4 border-orange-400">
              <img
                src="/api/placeholder/400/400"
                alt="Profile"
                className="w-full h-full object-cover"
              />
            </div>
          </div>

          {/* Skills Section */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-orange-400">
            <h2 className="text-xl font-bold mb-4 text-orange-600">ทักษะและความสามารถ</h2>
            <div className="space-y-2">
              <SkillBar label="การแก้ไขปัญหา" value={90} color="orange" />
              <SkillBar label="ความคิดสร้างสรรค์" value={85} color="orange" />
              <SkillBar label="การทำงานเป็นทีม" value={95} color="orange" />
            </div>
          </div>

          {/* Language Skills */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-blue-400">
            <h2 className="text-xl font-bold mb-4 text-blue-600">ทักษะด้านภาษา</h2>
            <div className="space-y-2">
              <SkillBar label="C" value={75} color="blue" />
              <SkillBar label="JAVA" value={70} color="blue" />
            </div>
          </div>

          {/* Software Skills */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-purple-400">
            <h2 className="text-xl font-bold mb-4 text-purple-600">โปรแกรมที่ถนัด</h2>
            <div className="space-y-2">
              <SkillBar label="Photo shop" value={80} color="purple" />
              <SkillBar label="Canva" value={85} color="purple" />
              <SkillBar label="Microsoft (Word,Excel)" value={75} color="purple" />
            </div>
          </div>
        </div>

        {/* Right Column */}
        <div className="space-y-6">
          {/* Header */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-6 shadow-lg border-l-4 border-orange-400">
            <h1 className="text-4xl font-bold mb-4 bg-gradient-to-r from-orange-600 to-red-600 text-transparent bg-clip-text">
              รัชชานนท์ คำสัตย์
            </h1>
            <h2 className="text-xl text-orange-600 font-semibold">DEVERLOPER</h2>
          </div>

          {/* Profile */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-blue-400">
            <h2 className="text-xl font-bold mb-2 text-blue-600">โปรไฟล์</h2>
            <p className="text-gray-700">
              I am studying and practicing coding skills at the undergraduate level. It focuses on developing and creating an understanding of the basics of program development. as well as solving problems with various coding languages to prepare for the application of knowledge in related fields in the future.
            </p>
          </div>

          {/* Contact */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-green-400">
            <h2 className="text-xl font-bold mb-4 text-green-600">ช่องทางการติดต่อ</h2>
            <div className="space-y-2">
              <div className="flex items-center gap-2 hover:text-green-600 transition-colors">
                <Phone size={20} className="text-green-500" />
                <span>080-146-1604</span>
              </div>
              <div className="flex items-center gap-2 hover:text-green-600 transition-colors">
                <Mail size={20} className="text-green-500" />
                <span>66025234@up.ac.th</span>
              </div>
              <div className="flex items-center gap-2 hover:text-green-600 transition-colors">
                <Home size={20} className="text-green-500" />
                <span>54 หมู่ 3 ต.บ้านโฮ่ง อ.ลาดยาว จ.นครสวรรค์ 60150</span>
              </div>
            </div>
          </div>

          {/* Education */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-yellow-400">
            <h2 className="text-xl font-bold mb-4 text-yellow-600">การศึกษา</h2>
            <div className="space-y-4">
              <div className="flex gap-4">
                <div className="w-2 bg-yellow-200 relative">
                  <div className="absolute w-3 h-3 bg-yellow-400 rounded-full -left-0.5" />
                </div>
                <div>
                  <div className="font-bold text-yellow-700">2017 - 2020</div>
                  <div>โรงเรียนลาดยาววิทยาคม</div>
                  <div className="text-gray-600">สายวิทย์ - คณิต</div>
                </div>
              </div>
              <div className="flex gap-4">
                <div className="w-2 bg-yellow-200 relative">
                  <div className="absolute w-3 h-3 bg-yellow-400 rounded-full -left-0.5" />
                </div>
                <div>
                  <div className="font-bold text-yellow-700">2023 - 2024</div>
                  <div>ปริญญาตรี มหาวิทยาลัยพะเยา</div>
                  <div className="text-gray-600">สาขา Computer since</div>
                </div>
              </div>
            </div>
          </div>

          {/* Hobbies */}
          <div className="bg-white/80 backdrop-blur-sm rounded-lg p-4 shadow-lg border-l-4 border-red-400">
            <h2 className="text-xl font-bold mb-4 text-red-600">งานอดิเรก</h2>
            <div className="space-y-2">
              <SkillBar label="กีฬา" value={80} color="red" />
              <SkillBar label="ดูหนัง" value={70} color="red" />
              <SkillBar label="เล่นเกมส์" value={90} color="red" />
            </div>
          </div>
        </div>
      </div>
    </div>
  );
};

const SkillBar = ({ label, value, color }) => {
  const getColorClasses = (color) => {
    const colors = {
      orange: "bg-orange-500",
      blue: "bg-blue-500",
      purple: "bg-purple-500",
      red: "bg-red-500",
    };
    return colors[color] || colors.orange;
  };

  return (
    <div className="space-y-1">
      <div className="flex justify-between">
        <span className="font-medium">{label}</span>
      </div>
      <div className="h-2 bg-gray-200 rounded-full overflow-hidden">
        <div 
          className={`h-full rounded-full transition-all duration-500 ${getColorClasses(color)}`}
          style={{ width: `${value}%` }}
        />
      </div>
    </div>
  );
};

export default DeveloperProfile;
