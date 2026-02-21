import React, { useState, useEffect } from "react";
import { Card, CardContent } from "@/components/ui/card";
import { Button } from "@/components/ui/button";
import { Input } from "@/components/ui/input";
import { Textarea } from "@/components/ui/textarea";
import { motion } from "framer-motion";

export default function AutoescuelaApp() {
  const [view, setView] = useState("admin");
  const [password, setPassword] = useState("");
  const [isAuthenticated, setIsAuthenticated] = useState(false);

  // Estados principales
  const [students, setStudents] = useState([]);
  const [lessons, setLessons] = useState([]);
  const [payments, setPayments] = useState([]);
  const [announcements, setAnnouncements] = useState([]);

  // Formularios
  const [studentName, setStudentName] = useState("");
  const [studentPhone, setStudentPhone] = useState("");
  const [lessonStudent, setLessonStudent] = useState("");
  const [lessonDate, setLessonDate] = useState("");
  const [paymentStudent, setPaymentStudent] = useState("");
  const [paymentAmount, setPaymentAmount] = useState("");
  const [announcementText, setAnnouncementText] = useState("");

  // Guardar en localStorage
  useEffect(() => {
    const data = localStorage.getItem("autoescuelaData");
    if (data) {
      const parsed = JSON.parse(data);
      setStudents(parsed.students || []);
      setLessons(parsed.lessons || []);
      setPayments(parsed.payments || []);
      setAnnouncements(parsed.announcements || []);
    }
  }, []);

  useEffect(() => {
    localStorage.setItem(
      "autoescuelaData",
      JSON.stringify({ students, lessons, payments, announcements })
    );
  }, [students, lessons, payments, announcements]);

  const login = () => {
    if (password === "admin123") {
      setIsAuthenticated(true);
    }
  };

  const addStudent = () => {
    if (!studentName) return;
    setStudents([...students, { name: studentName, phone: studentPhone }]);
    setStudentName("");
    setStudentPhone("");
  };

  const addLesson = () => {
    if (!lessonStudent || !lessonDate) return;
    setLessons([...lessons, { student: lessonStudent, date: lessonDate }]);
    setLessonStudent("");
    setLessonDate("");
  };

  const addPayment = () => {
    if (!paymentStudent || !paymentAmount) return;
    setPayments([
      ...payments,
      { student: paymentStudent, amount: paymentAmount },
    ]);
    setPaymentStudent("");
    setPaymentAmount("");
  };

  const addAnnouncement = () => {
    if (!announcementText) return;
    setAnnouncements([...announcements, announcementText]);
    setAnnouncementText("");
  };

  return (
    <div className="min-h-screen bg-gray-100 p-6">
      <motion.h1
        initial={{ opacity: 0, y: -20 }}
        animate={{ opacity: 1, y: 0 }}
        className="text-3xl font-bold text-center mb-6"
      >
        Autoescuela Online
      </motion.h1>

      <div className="flex justify-center gap-4 mb-6">
        <Button onClick={() => setView("admin")} className="rounded-2xl">
          Administrador
        </Button>
        <Button onClick={() => setView("public")} className="rounded-2xl">
          Versión Pública
        </Button>
      </div>

      {view === "admin" && !isAuthenticated && (
        <Card className="max-w-md mx-auto rounded-2xl shadow-lg">
          <CardContent className="p-6 space-y-4">
            <h2 className="text-xl font-semibold">Acceso Administrador</h2>
            <Input
              type="password"
              placeholder="Contraseña"
              value={password}
              onChange={(e) => setPassword(e.target.value)}
            />
            <Button onClick={login} className="w-full rounded-2xl">
              Entrar
            </Button>
            <p className="text-sm text-gray-500">
              Contraseña por defecto: admin123
            </p>
          </CardContent>
        </Card>
      )}

      {view === "admin" && isAuthenticated && (
        <div className="grid md:grid-cols-2 gap-6">
          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Gestión de Alumnos</h2>
              <Input placeholder="Nombre" value={studentName} onChange={(e) => setStudentName(e.target.value)} />
              <Input placeholder="Teléfono" value={studentPhone} onChange={(e) => setStudentPhone(e.target.value)} />
              <Button onClick={addStudent} className="w-full rounded-2xl">Añadir</Button>
              {students.map((s, i) => (
                <div key={i} className="bg-white p-2 rounded-xl shadow">{s.name} - {s.phone}</div>
              ))}
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Clases Prácticas</h2>
              <Input placeholder="Alumno" value={lessonStudent} onChange={(e) => setLessonStudent(e.target.value)} />
              <Input type="datetime-local" value={lessonDate} onChange={(e) => setLessonDate(e.target.value)} />
              <Button onClick={addLesson} className="w-full rounded-2xl">Programar</Button>
              {lessons.map((l, i) => (
                <div key={i} className="bg-white p-2 rounded-xl shadow">
                  {l.student} - {new Date(l.date).toLocaleString()}
                </div>
              ))}
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Control de Pagos</h2>
              <Input placeholder="Alumno" value={paymentStudent} onChange={(e) => setPaymentStudent(e.target.value)} />
              <Input type="number" placeholder="Cantidad €" value={paymentAmount} onChange={(e) => setPaymentAmount(e.target.value)} />
              <Button onClick={addPayment} className="w-full rounded-2xl">Registrar</Button>
              {payments.map((p, i) => (
                <div key={i} className="bg-white p-2 rounded-xl shadow">
                  {p.student} - {p.amount} €
                </div>
              ))}
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6 space-y-4">
              <h2 className="text-xl font-semibold">Avisos Públicos</h2>
              <Textarea placeholder="Escribe un aviso" value={announcementText} onChange={(e) => setAnnouncementText(e.target.value)} />
              <Button onClick={addAnnouncement} className="w-full rounded-2xl">Publicar</Button>
            </CardContent>
          </Card>
        </div>
      )}

      {view === "public" && (
        <div className="max-w-3xl mx-auto space-y-6">
          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold mb-4">Avisos</h2>
              {announcements.map((a, i) => (
                <div key={i} className="bg-white p-3 rounded-xl shadow mb-2">{a}</div>
              ))}
            </CardContent>
          </Card>

          <Card className="rounded-2xl shadow-lg">
            <CardContent className="p-6">
              <h2 className="text-2xl font-semibold mb-4">Próximas Clases</h2>
              {lessons.map((l, i) => (
                <div key={i} className="bg-white p-3 rounded-xl shadow mb-2">
                  {l.student} - {new Date(l.date).toLocaleString()}
                </div>
              ))}
            </CardContent>
          </Card>
        </div>
      )}
    </div>
  );
}
