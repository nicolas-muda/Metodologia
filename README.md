# Metodologia

-- PERSONAL

INSERT INTO personal (user, password, tipo, nombre) 
VALUES ('ema98','1234',0,'Emanuel'),
('fran67','1234',0,'Frank'),
('jacket','1234',0,'Jacquette'), 
('cletus','1234',0,'Cletus'), 
('seymurr','1234',0,'Seymour'), 
('claibyn','1234',0,'Claiborn'), 
('amenier','1234',1,'Annemarie'), 
('eleanor','1234',1,'Eleanor'), 
('farlin','1234',1,'Farlie'), 
('ferdina','1234',0,'Ferdinanda');

-- SECRETARIO

INSERT INTO secretario (user) 
VALUES ('amenier'), ('eleanor'), ('farlin');

-- MEDICA

INSERT INTO medica (especialidad,obra_social,personal_user,secretario_personal_user) 
VALUES ('Psiquiatría','IOMA','ema98','amenier'), ('Pediatría','OSDE','fran67','amenier'), ('Geriatría','IOMA','jacket','eleanor'), ('Cardiología','OSECAC','cletus','eleanor'), ('Pediatría','AVALANT','seymurr','eleanor'), ('Rehabilitación','OSDE','claibyn','farlin'), ('Cardiología','OSDE','ferdina','farlin');

-- PACIENTE

INSERT INTO paciente (dni, nombre, apellido, direccion, telefono, email, obra_social, nro_afiliado) 
VALUES ('57434950','Egor','Streatley','028 Pennsylvania Circle','9484666010','estreatley0@goo.ne','IOMA','1'), 
('10556659','Olivette','Banger','2020 Fairview Place','4982871298','obanger1@irs.gov','OSDE','2'), 
('41422393','Tiffany','Dresse','3030 Garrison Center','8895118528','tdresse2@fema.gov','IOMA','3'), 
('16604723','Prescott','Jostan','0 Troy Point','1358814587','pjostan3@1und1.de','OSDE','4'), 
('15398165','Rafael','Ellingham','562 Comanche Circle','7061233509','rellingham4@bandcamp.com','OSECAC','5'), 
('21491392','Ollie','Arderne','6122 Village Road','4233642979','oarderne5@tamu.edu','AVALANT','6'), 
('75483944','Pasquale','Pogue','1584 Little Fleur Pass','6516103428','ppogue6@irs.gov','OSDE','7'), 
('61012688','Odo','Missington','116 Monica Trail','5844831464','omissington7@about.me','IOMA','8'), 
('14036504','Anabelle','Wetherick','09 Nelson Plaza','1101057437','awetherick8@ed.gov','AVALANT','9'), 
('18577496','Matilda','Lewcock','0463 Dexter Lane','6703982163','mlewcock9@wsj.com','IOMA','10');

-- TURNOS

INSERT INTO turnos (paciente_dni,fecha,hora,turno,medica_personal_user) 
VALUES (57434950,'18/10/2022','11:00','m','ema98'), 
(57434950,'20/10/2022','13:00','t','ema98'), 
(10556659,'20/10/2022','15:50','t','fran67'), 
(10556659,'22/10/2022,10:00','m','claibyn'), 
(41422393,'29/10/2022','09:30','m','jacket'), 
(41422393,'30/10/2022','17:25','t','ferdina'), 
(16604723,'30/10/2022,18:00','t','fran67'), 
(16604723,'01/11/2022,07:00','m','seymurr'), 
(15398165,'12/11/2022,13:20','t','claibyn'), 
(15398165,'15/11/2022,08:55','t','seymurr'), 
(21491392,'16/11/2022,06:50','m','seymurr'), 
(21491392,'18/11/2022,10:10','m','cletus'), 
(75483944,'19/11/2022,09:20','m','cletus'), 
(75483944,'20/11/2022,08:50','m','cletus'), 
(61012688,'20/11/2022,16:55','t','seymurr'),
(61012688,'18/10/2022,11:00','m','ema98'), 
(14036504,'20/10/2022,13:00','t','ema98'), 
(14036504,'20/10/2022,15:50','t','fran67'), 
(18577496,'22/10/2022,10:00','m','claibyn'), 
(18577496,'29/10/2022,09:30','m','jacket'), 
(18577496,'30/10/2022,17:25','t','ferdina');
