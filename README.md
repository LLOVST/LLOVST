import React, { useState, useEffect } from 'react';

const MyGitHubProfile = () => {
  const [age, setAge] = useState(0);

  useEffect(() => {
    const calculateAge = () => {
      const today = new Date();
      const birthDate = new Date('2004-06-11');
      const yearsDiff = today.getFullYear() - birthDate.getFullYear();
      const monthsDiff = today.getMonth() - birthDate.getMonth();

      
    return () => clearInterval(interval);
  }, []);

  return (
    <div className="p-6 bg-gray-100 rounded-lg shadow-md">
      <h2 className="text-2xl font-bold mb-4">About Me</h2>
      <p className="text-lg mb-2">Age: {age} years</p>
      <p className="text-lg mb-4">Born on: June 11, 2004</p>
      <h3 className="text-xl font-bold mb-2">Skills</h3>
      <ul className="list-disc pl-6">
        <li>JavaScript</li>
        <li>React</li>
        <li>Node.js</li>
        <li>Python</li>
        <li>SQL</li>
      </ul>
    </div>
  );
};

export default MyGitHubProfile;
