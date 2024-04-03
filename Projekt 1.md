# Project-1
-- Prosty projekt modelu bazy danych zapisu studentó na wybrane kursy oferowane przez uczelnię, mając do dyspozycji 3 tabele: studenci, zapisy, kursy

/* Tworzenie tabeli "Studenci"*/

CREATE TABLE Student (
    student_id INT PRIMARY KEY,
    imie VARCHAR(50),
    nazwisko VARCHAR(50),
    email VARCHAR(100),
    nr_indeksu VARCHAR(20) UNIQUE
);

/*Tworzenie tabeli "Kursy"*/

CREATE TABLE Kursy (
    kurs_id INT PRIMARY KEY,
    nazwa VARCHAR(100),
    prowadzacy VARCHAR(100),
    sala VARCHAR(20),
    godzina_rozpoczecia TIME,
    godzina_zakonczenia TIME
);

