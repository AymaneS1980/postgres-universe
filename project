--
-- PostgreSQL database dump
--

-- Dumped from database version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)
-- Dumped by pg_dump version 12.17 (Ubuntu 12.17-1.pgdg22.04+1)

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

DROP DATABASE universe;
--
-- Name: universe; Type: DATABASE; Schema: -; Owner: freecodecamp
--

CREATE DATABASE universe WITH TEMPLATE = template0 ENCODING = 'UTF8' LC_COLLATE = 'C.UTF-8' LC_CTYPE = 'C.UTF-8';


ALTER DATABASE universe OWNER TO freecodecamp;

\connect universe

SET statement_timeout = 0;
SET lock_timeout = 0;
SET idle_in_transaction_session_timeout = 0;
SET client_encoding = 'UTF8';
SET standard_conforming_strings = on;
SELECT pg_catalog.set_config('search_path', '', false);
SET check_function_bodies = false;
SET xmloption = content;
SET client_min_messages = warning;
SET row_security = off;

SET default_tablespace = '';

SET default_table_access_method = heap;

--
-- Name: blackhols; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.blackhols (
    blackhols_id integer NOT NULL,
    name character varying(255) NOT NULL,
    description text,
    blackhols_types text,
    age_in_millions_of_years numeric,
    galaxy_id integer,
    distance_from_earth_inlight_speed integer
);


ALTER TABLE public.blackhols OWNER TO freecodecamp;

--
-- Name: blackhols_blackhols_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.blackhols_blackhols_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.blackhols_blackhols_id_seq OWNER TO freecodecamp;

--
-- Name: blackhols_blackhols_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.blackhols_blackhols_id_seq OWNED BY public.blackhols.blackhols_id;


--
-- Name: galaxy; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.galaxy (
    galaxy_id integer NOT NULL,
    name character varying(255) NOT NULL,
    description text,
    galaxy_types text,
    age_in_millions_of_years numeric
);


ALTER TABLE public.galaxy OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.galaxy_galaxy_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.galaxy_galaxy_id_seq OWNER TO freecodecamp;

--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.galaxy_galaxy_id_seq OWNED BY public.galaxy.galaxy_id;


--
-- Name: moon; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.moon (
    moon_id integer NOT NULL,
    name character varying(255) NOT NULL,
    description text,
    moon_types text,
    age_in_millions_of_years numeric,
    is_spherical boolean DEFAULT true,
    planet_id integer
);


ALTER TABLE public.moon OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.moon_moon_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.moon_moon_id_seq OWNER TO freecodecamp;

--
-- Name: moon_moon_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.moon_moon_id_seq OWNED BY public.moon.moon_id;


--
-- Name: planet; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.planet (
    planet_id integer NOT NULL,
    name character varying(255) NOT NULL,
    description text,
    planet_types text,
    age_in_millions_of_years numeric,
    has_life boolean DEFAULT true,
    star_id integer,
    distance_from_earth_inlight_speed integer
);


ALTER TABLE public.planet OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.planet_planet_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.planet_planet_id_seq OWNER TO freecodecamp;

--
-- Name: planet_planet_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.planet_planet_id_seq OWNED BY public.planet.planet_id;


--
-- Name: star; Type: TABLE; Schema: public; Owner: freecodecamp
--

CREATE TABLE public.star (
    star_id integer NOT NULL,
    name character varying(255) NOT NULL,
    description text,
    star_types text,
    age_in_millions_of_years numeric,
    galaxy_id integer
);


ALTER TABLE public.star OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE; Schema: public; Owner: freecodecamp
--

CREATE SEQUENCE public.star_star_id_seq
    AS integer
    START WITH 1
    INCREMENT BY 1
    NO MINVALUE
    NO MAXVALUE
    CACHE 1;


ALTER TABLE public.star_star_id_seq OWNER TO freecodecamp;

--
-- Name: star_star_id_seq; Type: SEQUENCE OWNED BY; Schema: public; Owner: freecodecamp
--

ALTER SEQUENCE public.star_star_id_seq OWNED BY public.star.star_id;


--
-- Name: blackhols blackhols_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.blackhols ALTER COLUMN blackhols_id SET DEFAULT nextval('public.blackhols_blackhols_id_seq'::regclass);


--
-- Name: galaxy galaxy_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy ALTER COLUMN galaxy_id SET DEFAULT nextval('public.galaxy_galaxy_id_seq'::regclass);


--
-- Name: moon moon_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon ALTER COLUMN moon_id SET DEFAULT nextval('public.moon_moon_id_seq'::regclass);


--
-- Name: planet planet_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet ALTER COLUMN planet_id SET DEFAULT nextval('public.planet_planet_id_seq'::regclass);


--
-- Name: star star_id; Type: DEFAULT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star ALTER COLUMN star_id SET DEFAULT nextval('public.star_star_id_seq'::regclass);


--
-- Data for Name: blackhols; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.blackhols VALUES (1, 'Sagittarius A*', 'Supermassive', 'At the Milky Way’s center', 13000, NULL, NULL);
INSERT INTO public.blackhols VALUES (2, 'Cygnus X-1', 'Stellar', 'Binary system with a black hole', 5000, NULL, NULL);
INSERT INTO public.blackhols VALUES (3, 'M87*', 'Supermassive', 'Imaged by the Event Horizon Telescope', 13000, NULL, NULL);
INSERT INTO public.blackhols VALUES (4, 'TON 618', 'Ultra-Massive', 'One of the most massive known', 10400, NULL, NULL);


--
-- Data for Name: galaxy; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.galaxy VALUES (1, 'Milky Way', 'Our home galaxy with spiral arms', 'Spiral Galaxy', 13600);
INSERT INTO public.galaxy VALUES (3, 'Andromeda', 'Spiral Galaxy', 'Nearest large galaxy to Milky Way', 10000);
INSERT INTO public.galaxy VALUES (4, 'Messier 87', 'Contains a supermassive black hole', 'Elliptical', 13700);
INSERT INTO public.galaxy VALUES (5, 'Large Magellanic', 'Satellite galaxy of Milky Way', 'Dwarf Galaxy', 13000);
INSERT INTO public.galaxy VALUES (6, 'Sombrero Galaxy', 'Bright central bulge, ring of dust', 'Spiral Galaxy', 12000);
INSERT INTO public.galaxy VALUES (7, 'Whirlpool Galaxy (M51)', 'Famous spiral shape interacting with smaller galaxy', 'Spiral Galaxy', 13000);


--
-- Data for Name: moon; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.moon VALUES (2, 'Europa', 'Jupiter s moon may have subsurface ocean', 'Icy Moon', 4500, false, 1);
INSERT INTO public.moon VALUES (3, 'Titan', 'Saturn s moon with thick atmosphere', 'Large Moon', 4500, false, 1);
INSERT INTO public.moon VALUES (4, 'Phobos', 'Mars larger irregular moon', 'Small Moon', 4500, false, 1);
INSERT INTO public.moon VALUES (5, 'Ganymede', 'Largest moon in the Solar System', 'Icy Moon', 4500, false, 1);
INSERT INTO public.moon VALUES (6, 'Callisto', '2nd largest moon of ,Jupiter,heavily cratered', 'Icy Moon', 4500, false, 1);
INSERT INTO public.moon VALUES (7, 'Io', 'Most volcanically active body in Solar System', 'Volcanic Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (8, 'Enceladus', 'Shoots water vapor, possible subsurface ocean', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (9, 'Mimas', 'Saturn moon, resembles Death Star', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (10, 'Rhea', 'Saturn s 2nd largest moon, icy and cratered', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (11, 'Dione', 'Icy, with signs of tectonic activity', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (12, 'Tethys', 'Features a massive impact crater', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (13, 'Iapetus', 'Saturn moon with light/dark sides', 'Dual-tone Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (14, 'Oberon', 'One of Uranus largest moons', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (15, 'Titania', 'Largest moon of Uranus', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (16, 'Umbriel', 'Very dark surface, Uranus moon', 'Dark Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (17, 'Ariel', 'Smooth, bright Uranus moon', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (18, 'Miranda', 'Strange surface, Uranus smallest major moon', 'Patchwork Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (19, 'Triton', 'Neptune’s large moon, may be a captured object', 'Retrograde Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (20, 'Charon', 'Largest moon of Pluto, almost a twin in size', 'Icy Moon', 4500, true, 1);
INSERT INTO public.moon VALUES (1, 'Moon', 'Earth s only natural satellite', 'Natural Moon', 4500, false, 1);


--
-- Data for Name: planet; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.planet VALUES (2, 'Mars', 'May have had water', 'Terrestrial', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (3, 'Jupiter', 'Largest planet in Solar System', 'Gas Giant', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (4, 'Kepler-22b', 'Potentially habitable exoplanet', 'Exoplanet', 6000, true, 1, NULL);
INSERT INTO public.planet VALUES (5, 'Venus', 'Thick atmosphere, extreme heat', 'Terrestrial', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (6, 'Saturn', 'Known for its beautiful ring system', 'Gas Giant', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (7, 'Neptune', 'Farthest known planet in our Solar System', 'Ice Giant', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (8, 'Uranus', 'Rotates on its side; coldest planet', 'Ice Giant', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (9, 'Mercury', 'Closest planet to the Sun', 'Terrestrial', 4600, true, 1, NULL);
INSERT INTO public.planet VALUES (10, 'WASP-12b', 'Extremely hot exoplanet, very close to its star', 'Hot Jupiter', 0, true, 1, NULL);
INSERT INTO public.planet VALUES (11, 'TRAPPIST-1e', 'Earth-sized, possibly habitable', 'Exoplanet', 0, true, 1, NULL);
INSERT INTO public.planet VALUES (12, 'HD 209458 b', 'First exoplanet observed with atmosphere', 'Exoplanet', 0, true, 1, NULL);
INSERT INTO public.planet VALUES (1, 'Earth', 'Only known planet with life', 'Terrestrial', 4540, true, 1, NULL);


--
-- Data for Name: star; Type: TABLE DATA; Schema: public; Owner: freecodecamp
--

INSERT INTO public.star VALUES (2, 'Sirius A', 'Brightest star in the night sky', 'A-Type Star', 242, 1);
INSERT INTO public.star VALUES (3, 'Betelgeuse', 'Nearing end of life, variable size', 'Red Supergiant', 10, 1);
INSERT INTO public.star VALUES (4, 'Proxima C.', 'Closest star to the Sun', 'Red Dwarf', 4850, 1);
INSERT INTO public.star VALUES (5, 'Rigel', 'Bright and massive, short-lived star', 'Blue Supergiant', 8, 1);
INSERT INTO public.star VALUES (6, 'Vega', 'Very bright star in Lyra constellation', 'A-Type Star', 455, 1);
INSERT INTO public.star VALUES (1, 'Sun', 'Center of the Solar System', 'G-Type Star', 4600, 1);


--
-- Name: blackhols_blackhols_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.blackhols_blackhols_id_seq', 4, true);


--
-- Name: galaxy_galaxy_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.galaxy_galaxy_id_seq', 13, true);


--
-- Name: moon_moon_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.moon_moon_id_seq', 20, true);


--
-- Name: planet_planet_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.planet_planet_id_seq', 12, true);


--
-- Name: star_star_id_seq; Type: SEQUENCE SET; Schema: public; Owner: freecodecamp
--

SELECT pg_catalog.setval('public.star_star_id_seq', 6, true);


--
-- Name: blackhols blackhols_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.blackhols
    ADD CONSTRAINT blackhols_name_key UNIQUE (name);


--
-- Name: blackhols blackhols_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.blackhols
    ADD CONSTRAINT blackhols_pkey PRIMARY KEY (blackhols_id);


--
-- Name: galaxy galaxy_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_name_key UNIQUE (name);


--
-- Name: galaxy galaxy_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.galaxy
    ADD CONSTRAINT galaxy_pkey PRIMARY KEY (galaxy_id);


--
-- Name: moon moon_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_name_key UNIQUE (name);


--
-- Name: moon moon_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT moon_pkey PRIMARY KEY (moon_id);


--
-- Name: planet planet_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_name_key UNIQUE (name);


--
-- Name: planet planet_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT planet_pkey PRIMARY KEY (planet_id);


--
-- Name: star star_name_key; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_name_key UNIQUE (name);


--
-- Name: star star_pkey; Type: CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT star_pkey PRIMARY KEY (star_id);


--
-- Name: star fk_galaxy; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.star
    ADD CONSTRAINT fk_galaxy FOREIGN KEY (galaxy_id) REFERENCES public.galaxy(galaxy_id);


--
-- Name: moon fk_planet; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.moon
    ADD CONSTRAINT fk_planet FOREIGN KEY (planet_id) REFERENCES public.planet(planet_id);


--
-- Name: planet fk_star; Type: FK CONSTRAINT; Schema: public; Owner: freecodecamp
--

ALTER TABLE ONLY public.planet
    ADD CONSTRAINT fk_star FOREIGN KEY (star_id) REFERENCES public.star(star_id);


--
-- PostgreSQL database dump complete
--

