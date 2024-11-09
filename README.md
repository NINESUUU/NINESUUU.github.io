import React from 'react';
import { Phone, Mail, Home } from 'lucide-react';

const DeveloperProfile = () => {
  return (
    <div className="min-h-screen bg-white p-8 max-w-4xl mx-auto font-sans">
      <div className="grid grid-cols-1 md:grid-cols-2 gap-8">
        {/* Left Column */}
        <div className="space-y-6">
          {/* Profile Image */}
          <div className="relative">
            <div className="w-full aspect-square rounded-lg overflow-hidden">
              <img
                src="/api/placeholder/400/400"
                alt="Profile"
                className="w-full h-full object-cover"
              />
            </div>
          </div>

          {/* Skills Section */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">ทักษะและความสามารถ</h2>
            <div className="space-y-2">
              <SkillBar label="การแก้ไขปัญหา" value={90} />
              <SkillBar label="ความคิดสร้างสรรค์" value={85} />
              <SkillBar label="การทำงานเป็นทีม" value={95} />
            </div>
          </div>

          {/* Language Skills */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">ทักษะด้านภาษา</h2>
            <div className="space-y-2">
              <SkillBar label="C" value={75} />
              <SkillBar label="JAVA" value={70} />
            </div>
          </div>

          {/* Software Skills */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">โปรแกรมที่ถนัด</h2>
            <div className="space-y-2">
              <SkillBar label="Photo shop" value={80} />
              <SkillBar label="Canva" value={85} />
              <SkillBar label="Microsoft (Word,Excel)" value={75} />
            </div>
          </div>
        </div>

        {/* Right Column */}
        <div className="space-y-6">
          {/* Header */}
          <div>
            <h1 className="text-4xl font-bold mb-4">รัชชานนท์ คำสัตย์</h1>
            <h2 className="text-xl text-gray-600 mb-4">DEVERLOPER</h2>
          </div>

          {/* Profile */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-2">โปรไฟล์</h2>
            <p className="text-gray-700">
              I am studying and practicing coding skills at the undergraduate level. It focuses on developing and creating an understanding of the basics of program development. as well as solving problems with various coding languages to prepare for the application of knowledge in related fields in the future.
            </p>
          </div>

          {/* Contact */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">ช่องทางการติดต่อ</h2>
            <div className="space-y-2">
              <div className="flex items-center gap-2">
                <Phone size={20} />
                <span>080-146-1604</span>
              </div>
              <div className="flex items-center gap-2">
                <Mail size={20} />
                <span>66025234@up.ac.th</span>
              </div>
              <div className="flex items-center gap-2">
                <Home size={20} />
                <span>54 หมู่ 3 ต.บ้านโฮ่ง อ.ลาดยาว จ.นครสวรรค์ 60150</span>
              </div>
            </div>
          </div>

          {/* Education */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">การศึกษา</h2>
            <div className="space-y-4">
              <div className="flex gap-4">
                <div className="w-2 bg-gray-300 relative">
                  <div className="absolute w-3 h-3 bg-gray-500 rounded-full -left-0.5" />
                </div>
                <div>
                  <div className="font-bold">2017 - 2020</div>
                  <div>โรงเรียนลาดยาววิทยาคม</div>
                  <div className="text-gray-600">สายวิทย์ - คณิต</div>
                </div>
              </div>
              <div className="flex gap-4">
                <div className="w-2 bg-gray-300 relative">
                  <div className="absolute w-3 h-3 bg-gray-500 rounded-full -left-0.5" />
                </div>
                <div>
                  <div className="font-bold">2023 - 2024</div>
                  <div>ปริญญาตรี มหาวิทยาลัยพะเยา</div>
                  <div className="text-gray-600">สาขา Computer since</div>
                </div>
              </div>
            </div>
          </div>

          {/* Hobbies */}
          <div className="bg-[#f8e4d6] rounded-lg p-4">
            <h2 className="text-xl font-bold mb-4">งานอดิเรก</h2>
            <div className="space-y-2">
              <SkillBar label="กีฬา" value={80} />
              <SkillBar label="ดูหนัง" value={70} />
              <SkillBar label="เล่นเกมส์" value={90} />
            </div>
          </div>
        </div>
      </div>
    </div>
  );
};

const SkillBar = ({ label, value }) => {
  return (
    <div className="space-y-1">
      <div className="flex justify-between">
        <span>{label}</span>
      </div>
      <div className="h-2 bg-gray-200 rounded-full">
        <div 
          className="h-full bg-gray-600 rounded-full"
          style={{ width: `${value}%` }}
        />
      </div>
    </div>
  );
};

export default DeveloperProfile;
